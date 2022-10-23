# Today-I-Learned

##### 26/09/2022: Collection.stream().forEach() and Collection.forEach()
```
- The first difference between them is Execution Order. Collection.forEach() processed in order of the items. 
  In constract, the processing order of Collection.stream().forEach() is undefined. 
- The second thing is Modification. Collection.forEach() throws an exception immediately after removing an element. 
  In constrast, Collection.stream().forEach() continues interating over the whole list before see an exception. 
  In case of modifying, there is no problem with doing this using either Collection.stream().forEach() or Collection.forEach(), 
  but we shouldn't do this because the stream should facilitate parallel execution. 
  So, modifying elements of a stream could lead to unexpected behavior.
- Conclution: if we don't require a stream but only want to iterate over a collection, 
  the first choice should be using Collection.forEach() directly on the collection.
```
##### 27/09/2022: What is gRPC?
```

```
##### 29/09/2022: Why do we need api gate-way?
```

```
##### 30/09/2022: What is redis cache, spring cache?
```

```
##### 01/10/2022: group by, having in SQL?
```

```
##### 02/10/2022: How to check null in Java?
```

```
##### 03/10/2022: Serializable in Java?
```

```
##### 04/10/2022: ```&``` and ```&&``` in Java
```
- & evaluates both sides of the operation. 
- && evaluates the left side of the operation, if it's true, it continues and evaluates the right side. 
```
##### 09/10/2022: What is rebase in git?
```

```
##### 10/10/2022: Integer.toString() vs String.valueOf() in Java
```

```
##### 17/10/2022: What is BindingResult in Spring?
```
- BindingResult used as a parameter right after a Object that is being validated(use @Valid annotaion). 
- It hold the result of validation and contains errors that may have occured. 
- The BindingResult must come right after the model object is validated or else Spring will fail to validate the object and throw an exception.
```
##### 23/10/2022: RESTful APIs
```
API (Application Programing Interface)
- Major API categories: Local API and Remote API.
	+ Local API takes place in single computer.
	+ Remote API allow clients from a computer execute operation on another computer (sent over network using protocol)

- Remote API: Web APIs, SOAP service, RPC, Remote methods.
- Web APIs: REST, gPRC, GraphQL.
- RESTful APIs (Representational State Transfer): defines a set of constraints that describe how networked resources are difined for communications between clients and servers.
- REST Principles: Client-server based, Stateless, Cacheable, Layered, Uniform interface.
- Uniform Resource Identifier(URI): https://api.pets.com/api/v1/users/{userId}/pets/{petId}
	+ https: Protocol
	+ api.pets.com/ : Domain name
	+ api/v1: Entry Point
	+ users/ : Collection.
	+ {userId}, {petId} : Path Variable
	+ pets: Sub Collection.
- Resource Representation: JSON, XML.
- API Security: 
	+ Basic authentication: A username and password is provided with each request.
	+ API Keys: A unique generated value is assigned to each client and used for authentication.
	+ OAuth 2: A token-based appoach to authorization that supports various scenarios, including machine to machine and delegated access.
- API takeaways:
	+ API Clients send requests and receive responses via HTTP. 
	+ REST Principles will shape API calls and response handing.
	+ Security schemes must be taken into account.
- Java HTTP Client, Spring WebClient(webflux), RestTemplate, OpenFeign(feign-core, feign-jackson).
- API Interaction Approaches: Synchronous, Asynchronous, Streaming.
```
