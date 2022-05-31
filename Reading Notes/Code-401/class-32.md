# Class 32
## Reading

### [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

- Together with authentication and throttling, permissions determine whether a request should be granted or denied access
- Permission checks are always run at the very start of the view, before any other code is allowed to proceed
- Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted
- Permissions are used to grant or deny access for different classes of users to different parts of the API
- The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user
- This corresponds to the IsAuthenticated class in REST framework
- A slightly less strict style of permission would be to allow full access to authenticated users, but allow read-only access to unauthenticated users
- This corresponds to the IsAuthenticatedOrReadOnly class in REST framework
- Permissions in REST framework are always defined as a list of permission classes
- If any permission check fails, an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run
- Setting the permission policy:


    REST_FRAMEWORK = {
        'DEFAULT_PERMISSION_CLASSES': [
            'rest_framework.permissions.IsAuthenticated',
        ]
    }

  

## Bookmark and Review

### [Classy Django REST](http://www.cdrf.co/)

### [DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)