### Which HTTP method would you use to update a record through an API?
PUT. The PUT method is used to create or replace a resource.

### Which REST methods require an ID parameter?
DELETE. The ID parameter is required for methods that modify or delete resources.

### What’s the relationship between REST and CRUD?
 REST is an architectural style for designing APIs, while CRUD is a set of operations for manipulating data.
 
 ### If you had to describe the process of creating a RESTful API in 5 steps, what would they be?
 
- Define your resources. The first step is to define the resources that your API will expose. A resource is a data or functionality. For example, a resource could be a customer, an order, or a product.
- Determine the HTTP methods for each resource. Once you have defined your resources, you need to determine the HTTP methods that will be used to access them. The HTTP methods GET, POST, PUT, and DELETE are commonly used to create, read, update, and delete resources, respectively.
- Design the URIs for your resources. The URIs (Uniform Resource Identifiers) for your resources should be unique and easy to remember. They should also be consistent with the HTTP methods that are used to access them. For example, the URI for a customer resource might be /customers. The URI for a GET request to retrieve a customer might be /customers/12345.
- Define the data formats for your resources. The data formats for your resources should be consistent with the HTTP methods that are used to access them. For example, the data format for a GET request to retrieve a customer might be JSON.
- Implement your API. Once you have defined the resources, HTTP methods, URIs, and data formats for your API, you can implement it. There are many different ways to implement a RESTful API. Some popular options include using a web framework
