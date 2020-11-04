## Overview

An example project to test:

* Building an API in Springboot.
* CI/CD integration in jenkins.
* Creating a springboot application working with Docker, and hosting the result.

## Pre-requisites

* JDK 11+
* Docker

## Building

### Testing

`./gradlew test`

### Building (no tests)

`./gradlew assemble`

### Building (with tests)

`./gradlew build`

### Running in Docker

`./gradlew assemble docker dockerRun`

### Stopping Docker container

`./gradlew dockerStop`

## Using API

* get all rides - GET [/ride](http://localhost:8080/ride) to get a list of all the rides
* get specific ride - GET [/ride/${id}](http://localhost:8080/ride/1) to get a specific ride
* create ride - POST JSON to [/ride](http://localhost:8080/ride) to create a new ride 
