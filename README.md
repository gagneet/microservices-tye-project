# Type Project for development, testing and deploying Microservices (microservices-tye-project)

## Table of contents
* [General info](https://devblogs.microsoft.com/aspnet/introducing-project-tye/)
* [Technologies](#technologies)
* [Setup](#setup)

## General info
This project is simple Type Project taken from the Microsoft Blog.

## Technologies
Project is created with:
* Tye Version: 0.2.0-alpha.20258.3
* Project version: 0.0.1
* .NET Code library version: 3.1

## Deploy Redis

$ kubectl apply -f https://raw.githubusercontent.com/dotnet/tye/master/docs/tutorials/hello-tye/redis.yaml
$ tye deploy --interactive
$ kubectl port-forward svc/frontend 5000:80
$ tye undeploy --what-if

## Setup
To run this project, install it locally using npm:

```
$ cd ../microservices
$ tye run
