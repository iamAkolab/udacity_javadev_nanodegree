# Web Services
## What is a Web Service?
A web service is a way to share data between two disparate systems. The communication typically happens between a client and a server.
* Client - The client makes a request for data.
* Server - The server responds to the client's request.

## Web Service Communication
The means of communication between the client and server is via a standard web protocol like HTTP (or HTTPS) on the world wide web, that uses a common language like JSON or XML.

A client invokes a web service by sending an XML (or JSON) message, then waits for a corresponding XML response from the server.

## How Web Services Work
* Step 1: The web service provider (the person who created the web service) defines a standard format for requests and also for the responses provided.
* Step 2: The client sends a request to the web service across the network.
* Step 3: The web service receives the request and performs an action (like query a database or perform a calculation) and sends a response back to the calling client.

# Benefits of Web Services
The concepts of reusability and usability allow organizations to use web services provided by third parties. This reduces development time and delivers more powerful applications.
* Revealing the Existing Function on Framework. ...
* Interoperability. ...
* Ordered Protocol. ...
* Ease of Use. ...
* Re-Ease of Use. ...
Send Capacity. ...
Agility. ...
Quality.

# Web Services vs APIs vs Microservices
Web Services started in the early 90's, the complexiities of SOAP based web service led to REST based API
API and Microservices are an evolution of web services. API allows for data sharing between two different applications or systems. APIs are more lightweight and streamlined and good for devices with limited bandwiths. One of the most obvious differences is that web services, unlike APIs, require a network to function. APIs can function online or offline.

Furthermore, web services are not protocol-agnostic like APIs. APIs can use any design style or protocol, but web services are restricted mostly to SOAP or Simple Object Access Protocol.

All web services are APIs but not all web APIs are web services.


While APIs and Webs Services are the communication interface for different architecture styles, microservices is a distinctive method to develop software systems that have well-defined interfaces and operability.
Micorserveice are fully contained, individual component that communicated to each other and call one client and are modeled around one specific business domain. e.g location microservice

## Publicly Accessible API

A list of publicly accessible APIs: https://github.com/public-apis/public-apis/blob/master/README.md.


