# Class 28
## Reading

### [Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)
- Django Forms take a lot of the work out of creating forms
- By providing a framework that lets you define forms and their fields programmatically
- Create forms.py:


    import datetime
    
    from django import forms
    
    from django.core.exceptions import ValidationError
    from django.utils.translation import gettext_lazy as _

    class RenewBookForm(forms.Form):
        renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")

    def clean_renewal_date(self):
        data = self.cleaned_data['renewal_date']

        # Check if a date is not in the past.
        if data < datetime.date.today():
            raise ValidationError(_('Invalid date - renewal in past'))

        # Check if a date is in the allowed range (+4 weeks from today).
        if data > datetime.date.today() + datetime.timedelta(weeks=4):
            raise ValidationError(_('Invalid date - renewal more than 4 weeks ahead'))

        # Remember to always return the cleaned data.
        return data
- There are many other types of form fields, which you will largely recognize from their similarity to the equivalent model field classes: 
- BooleanField, CharField, ChoiceField, TypedChoiceField, DateField, DateTimeField, DecimalField, DurationField, EmailField, FileField, 
- FilePathField, FloatField, ImageField, IntegerField, GenericIPAddressField, MultipleChoiceField, TypedMultipleChoiceField, NullBooleanField, 
- RegexField, SlugField, TimeField, URLField, UUIDField, ComboField, MultiValueField, SplitDateTimeField, ModelMultipleChoiceField, ModelChoiceField.
- URL Configuration:
  

    urlpatterns += [
        path('book/<uuid:pk>/renew/', views.renew_book_librarian, name='renew-book-librarian'),
    ]

- View:


    import datetime
    
    from django.shortcuts import render, get_object_or_404
    from django.http import HttpResponseRedirect
    from django.urls import reverse
    
    from catalog.forms import RenewBookForm
    
    def renew_book_librarian(request, pk):
        book_instance = get_object_or_404(BookInstance, pk=pk)
    
    # If this is a POST request then process the Form data
    if request.method == 'POST':

        # Create a form instance and populate it with data from the request (binding):
        form = RenewBookForm(request.POST)

        # Check if the form is valid:
        if form.is_valid():
            # process the data in form.cleaned_data as required (here we just write it to the model due_back field)
            book_instance.due_back = form.cleaned_data['renewal_date']
            book_instance.save()

            # redirect to a new URL:
            return HttpResponseRedirect(reverse('all-borrowed') )

    # If this is a GET (or any other method) create the default form.
    else:
        proposed_renewal_date = datetime.date.today() + datetime.timedelta(weeks=3)
        form = RenewBookForm(initial={'renewal_date': proposed_renewal_date})

    context = {
        'form': form,
        'book_instance': book_instance,
    }

    return render(request, 'catalog/book_renew_librarian.html', context)

- Template:


    {% extends "base_generic.html" %}
    
    {% block content %}
      <h1>Renew: {{ book_instance.book.title }}</h1>
      <p>Borrower: {{ book_instance.borrower }}</p>
      <p{% if book_instance.is_overdue %} class="text-danger"{% endif %}>Due date: {{ book_instance.due_back }}</p>
    
      <form action="" method="post">
        {% csrf_token %}
        <table>
        {{ form.as_table }}
        </table>
        <input type="submit" value="Submit">
      </form>
    {% endblock %}



## Bookmark and Review

### [Django Templates](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)

### [Django Views](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)