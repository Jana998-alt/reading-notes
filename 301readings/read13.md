# Read13: CRUD

## Status Codes Based On REST Methods

In your own words, describe what each group of status code represents:

100’s = Informational status codes; it tells information about the status of the code. 

200’s = Success codes. meaning that the request fulfiled all conditions required to process it. 

300’s = Redirection codes. the requested resource is not available any more. 

400’s = Client error codes. the request it self is not valid. for different reasons.

500’s =Server error codes. problems from server side, or wrong request from client that causes errors on the server side. 


What is a status code 202? 

used for  for asynchronous processing. it tells the client that the request is valid and being processed, but the result will be sent in some time in the future. 

What is a status code 308?

Permanent Redirect. when the resource url has changed, use this code.

What code would you use if an update didn’t return data to a client?

204 No Content.

What code would you use if a resource used to exist but no longer does?

410 Gone.

What is the ‘Forbidden’ status code?

403



## Build A REST API With Node.js, Express, & MongoDB - Quick 
_from Web Dev simplified_

- Why do we need to pull our MongoDB database string out of our server and put it into our .env?

because when we want to deploy our website, it can't use the local host. instead, it will use a variable from the invironment. 

- What is middleware?

a code that runs, once the server gets the request but before it passes to the route.

- What does app.use(express.json()) do?

lets our server to accept json as an element inside the body inside of an element (post, get ...)

- What does the /:id mean in a route?

this means that id is a parameter.

- What is the difference beween PUT and PATCH?

put updates all information about the user all at once, but patch updates the things that we want only.

- How do you make a defalut value in a schema?

add a property: _default_ in the object, and give it a default value.

- What does a 500 error status code mean?

means that there is an error in the server.

- What is the difference between a status 200 and a status 201?

200 : success in general.
201 : more specific: succesfuly sent an object.




## Things I want to know more about

- I want to learn more about schema
