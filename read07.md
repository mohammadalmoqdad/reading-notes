1. What’s the difference between PUT and PATCH?
- The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
* [Nock]('https://github.com/nock/nock')
* [MockServer]('https://www.mock-server.com')
* [Beeceptor]('https://beeceptor.com')

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?
* Client errors (400–499)
* Server errors (500–599)

4. Compare and contrast SOAP and ReST
- Simple Object Access Protocol(SOAP) and Representational State Transfer (REST) are by far the most used options for accessing web services, however they are not directly comparable as they vary in the sense that SOAP is a communications protocol while REST is a set of architectural principles for data transmission and SOAP is a messaging protocol for exchanging information between two computers based on XML over the internet. SOAP messages are purely written in XML which is why they are platform and language independent.

* **SOAP** The Simple Object Access Protocol (SOAP) is an XML-based protocol to let applications exchange information over HTTP.


* **ReST vaerbs** The Socrata API follows the REST (REpresentational State Transfer) design pattern. This means that the CRUD (Create, Read, Update, and Delete) operations are specified by using HTTP methods. These are referred to as RESTful verbs


* **CRUD VERBs** : update, or destroy instead of delete.

* **SWAGGER** : is an Interface Description Language for describing RESTful APIs expressed using JSON.


