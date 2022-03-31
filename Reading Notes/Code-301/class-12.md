# Class 12

## [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

### In your own words, describe what each group of status code represents

      100’s = The request will fail before sending
      200’s = Success!!
      300’s = The source was redirected
      400’s = Bad URL
      500’s = Server down

### What is a status code 202?

      Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

### What is a status code 308?

      Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

### What code would you use if an update didn’t return data to a client?

      204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

### What code would you use if a resource used to exist but no longer does?

      204 No Content - The most fitting status code for this case. It’s better to reduce traffic and simply tell the client the deletion is complete and return no response body (as the resource has been deleted).

### What is the ‘Forbidden’ status code?

      403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Video

[Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

    To Hide the credentials

### What is middleware?

    Software that enables connectivity between applications

### What does app.use(express.json()) do?

    Sends the json data to the server

### What does the /:id mean in a route?

    it gives you access to whatever you put after the slash

### What is the difference between PUT and PATCH?

    We only want to update based on what the user passes us. if we use put it would update all of the information to the subscriber all at once

### How do you make a default value in a schema?

    default: 

### What does a 500 error status code mean?

    500 – Internal Server Error, sometime's momentarily

### What is the difference between a status 200 and a status 201?

    200 – OK (you will see this one the most)
    201 – Created (a more specific way of saying successful )
