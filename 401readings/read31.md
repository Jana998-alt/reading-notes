# Django REST Framework & Docker

## Beginner’s Guide to Docker

Docker is a software that isolates the environment of the app. I beats the problem of different operating systems, and the coolest thing is that it can be shared between people! 
Now the problem is that it is complicated.
Using a virtual environment uses up space and CPU reasorses, so, they invented another way of isolation which is: *containers*.

docker uses containers. they are more light-weight on the device. 

*This, fundamentally, is what Docker is. A way to implement Linux containers!*

Two main concepts in docker: an image, and a container. 
An image is a snapshot in time of what a project contains. A container is a running instance of the image.

A baking analogy we can use here to show the general approach of docker:

- A Dockerfile is the recipe for a cake
- An image is a snapshot of the recipe at a given time
- A docker-compose.yml says how to make the cake
- And the container is the actual, baked cake
