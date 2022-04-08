# WebGoat 8 Spring Boot Web App Fuzzing Example with

## Introduction

Ci-Fuzz is a security suite with code coverage guided fuzzing at its core.

WebGoat is a deliberately insecure web application maintained by [OWASP](http://www.owasp.org/) designed to teach web
application security lessons.

This repository is a merge of WebGoat and the [Web App Fuzzing template](https://github.com/ci-fuzz/web-app-fuzzing-template-project) of @ci-fuzz

### Prerequisites:

* Java 17
* 
* Git, or Git support in your IDE

Open a command shell/window:

```Shell
git clone git@github.com:WebGoat/WebGoat.git
```

Now let's start by compiling the project.

```Shell
cd WebGoat
git checkout <<branch_name>>
# On Linux/Mac:
./mvnw clean install 
# On Windows:
./mvnw.cmd clean install
```

Now we are ready to run the project. WebGoat 8.x is using Spring-Boot.

```Shell
# On Linux/Mac:
./mvnw -pl webgoat-server spring-boot:run
# On Widows:
./mvnw.cmd -pl webgoat-server spring-boot:run

```
... you should be running WebGoat on localhost:8080/WebGoat momentarily


To change the IP address add the following variable to the `WebGoat/webgoat-container/src/main/resources/application.properties file`:

```
server.address=x.x.x.x
```
