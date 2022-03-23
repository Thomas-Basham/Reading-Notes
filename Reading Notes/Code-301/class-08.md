# Class 08

## [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

### What does REST stand for?

    Representational State Transfer

### REST APIs are designed around a ____

    Resource

### What is an identifer of a resource? Give an example

    Any kind of object data {"orderId":1,"orderValue":99.90,"productId":1,"quantity":1}

### What are the most common HTTP verbs?

    GET, POST, PUT, PATCH, and DELETE

### What should the URIs be based on?

    The resource

### Give an example of a good URI

    https://adventure-works.com/orders

### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

    An API that exposes a large number of small resources

### What status code does a successful GET request return?

    A successful GET method typically returns HTTP status code 200 (OK)    

### What status code does an unsuccessful GET request return?

    If the server cannot match any of the media type(s) listed, it should return HTTP status code 406 (Not Acceptable)

### What status code does a successful POST request return?

    A successful GET method typically returns HTTP status code 200 (OK)

### What status code does a successful DELETE request return?

    If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content),

## Bookmark/Skim

## [RegExr - Pay particular attention to the cheatsheet](https://regexr.com/)

### How would you match a phone number from your city using RegEx?

    Something to do with \d and digits 0-9

  [Regex Tutorial](https://regexr.com/)
  [Regex 101](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
