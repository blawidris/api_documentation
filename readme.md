# What is API

API simply means application program interface that sits between application and web server to act as intermediary layer that processes data transfer between systems. 

API can be defined as a set of rules that define how applications or devices can connect to and communicate with each other.

### How APIs work

When a client make a request to web server the following process is happens;

- Application initiates API call to retrieve information (know as request) via API's URI and includes a request verb (GET, POST, etc), headers and sometimes request body.
- After receiving a valid request the api makes a call to external program or web server
- Then the server send response to the API with requested information.
- The API now transfers the data to the initial requesting application.

**P.S**: Don't confuse API to UI as the two have different meaning. User interface (UI) is designed for use by human while API is design for use by computer or application.

### Why Use API?

- It offers security by design because their position as middleman facilitate the abstraction of functionality between two systems. API calls usually includes authorization credentials to reduce the risk of attacks on the server, and an API gateway can limit access to minimize security threats.
- It improves collaboration
- Easier innovation
- Data monetization

### Types of APIs

- Open APIs: it's an open source api that can be access with HTTP protocol. It is also known as public APIs.

- Partner APIs: These are public apis that can only be accessible when a developer provides a certain credentials. In order to get this credentials developer will have to complete an onboarding process e.g Twitter. Generally, Partner APIs is openly promoted but shared with business partners who have signed an agreement with the publisher.

- Internal APIs: these are private apis which are only available for users within an organization and are instead intended to improve productivity and communication across different internal development teams.

- Composite APIs (Combine multiple api):  It allows developer access several endpoints in a single call. It is useful in microservices architecture where performing a single task may require information from several sources.

### Types of protocol

- SOAP (Simple Object Access protocol)
    - It enables user to send and receive data through SMTP and HTTP. 
    - SOAP APIs easier to share information between software in different environment
    - SOAP APIs are mostly written in different environment
    - It relies solely on XML to provide messaging services

- XML-RPC
    - Relies on specific format of XML to transfer data
    - Simple and lightweight i.e uses minimal bandwidth

- REST (RESTful: Representational State Transfer)
    - It is a set of web API architecture principles and has no official standard unlike other protocols
    - uses four different HTTP 1.1 verbs (GET, POST, PUT, and DELETE) to perform tasks.
    - It response are based on Web services that output the data in Command Separated Value (CSV), JavaScript Object Notation (JSON) and Really Simple Syndication (RSS).

- JSON-RPC
    - Similar to XML-RPCs but it uses JSON format to transfer data

## What is REST API?

REST means representational state transfer, also know as RESTful API. It's an architecture style for designing networked applications which relies on stateless, client-server protocol and mostly HTTP.

It treats server objects as resources that can be created or destroy and can be used by virtually any programming language and support variety of data-formats. 


### REST Design Principles

- Statelessness: each request needs to include all the information necessary for processing it i.e doesn't require any server-side sessions as server applications are not allowed to store any data related to client request.

- Client-Server Decoupling
    - Client and server app must be completely independent of each 
    - Client app should only know the URI of the requested resource
    - Server application shouldn't modify the client application other than passing it to the requested data via HTTP

Other REST design principles includes;
- Uniform interface: 
- Code on demand
- Layered system architecture
- Cacheability

## HTTP METHODS

- GET: retrieve data from a specified resource
- POST: submit data to be processed by a specified resource
- DELETE: remove data from specified resource
- PUT: update data on specified resource
- PATCH: is used to make a partial update to a resource
- HEAD: unlike GET, HEAD does not send the response body but do send same headers.
- OPTIONS: allow communication between options for a given resource.
- TRACE: requests the server to send the exact request, as received by it, in the response body. It is useful for diagnostic purposes
- CONNECT: used to established end-to-end HTTP tunnel through proxy server

## What is API Endpoint

When an API interacts with another system, the touchpoints of this communication are considered endpoints. For APIs, an endpoint can include a URL of a server or service.

API endpoints are the specific digital location where requests for information are sent by one program to retrieve the digital resource that exists there i.e it's one end of a communication channel. 

An API's performance depends on its capacity to successfully communicate with API endpoints

APIs work using ‘requests’ and ‘responses.’ When an API requests information from a web application or web server, it will receive a response. The place that APIs send requests and where the resource lives, is called an endpoint.

example: http://localhost/products/list

**Reference Links**

- https://www.ibm.com/topics/api
- https://www.ibm.com/topics/rest-apis
- https://www.geeksforgeeks.org/explain-request-verbs/
- https://www.techtarget.com/searchapparchitecture/definition/API-endpoint#:~:text=Software%20programs%20typically%20have%20multiple,them%20to%20discover%20hashtagged%20media.