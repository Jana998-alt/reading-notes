# Read08

## API Design Best Practices

- What does REST stand for?

Representational State Transfer

REST APIs are designed around __resources__.

What is an identifer of a resource? Give an example.

URI that uniquely identifies that resource. for ecample: https://adventure-works.com/orders/1

What are the most common HTTP verbs?

GET, POST, PUT, PATCH, and DELETE.

What should the URIs be based on?

nouns 

Give an example of a good URI.

https://adventure-works.com/orders

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

web APIs that expose a large number of small resources, it is a bad thing because it makes a bigger load.

What status code does a successful GET request return?

status code 200

What status code does an unsuccessful GET request return?

404 (Not Found)

What status code does a successful POST request return?

status code 200 

What status code does a successful DELETE request return?

status code 204
