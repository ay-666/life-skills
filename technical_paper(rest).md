# Rest

So to understand rest first, like we should know how web services work. Like when a client wants something server its sends request to the server , and receives particular response in return.

So generally servers have some api endpoints for each different type of request to which the client sends request to for getting the response it wants.

Rest stands for Representational State Transfer. It's actually a simple set of rules for how web services should behave.
REST was created by Roy Fielding in 2000.These guidelines became known as the core principles of REST—six rules that define what makes an API "RESTful."

## The Core Principles of REST

### 1. Uniform Interface

This means APIs should work in a consistent, predictable way.
Example:

    GET /users/octocat          # Get user info
    GET /users/octocat/repos    # Get user's repositories   
    POST /user/repos  

The URLs (called "endpoints") clearly describe what resource we are working with, and the HTTP method (GET, POST, PATCH, DELETE) tells what action we want to perform.      

### 2. Stateless
Each request must contain all the information the server needs to understand and process it. The server doesn't remember anything about previous requests.

In the stateless version, each request includes the authentication token.
With stateless design, each request is independent. Any server can handle any request because all the information needed is contained in the request itself. This makes system more reliable, scalable, and easier to maintain.

### 3. Client-Server Separation
The client (app, web) and server (the API) are completely independent. We can update mobile app without changing the server, and vice versa.

### 4. Cacheable
Responses should clearly indicate whether they can be cached and for how long.

### 5. Layered System
A layered system means the architecture is organized in hierarchical layers, where each layer only knows about the layer directly below it. We don't need to know about any of this complexity—we just make our request to one URL, and the layered system handles the rest.

### 6. Code on Demand (Optional)

The server can send executable code to extend client functionality. This is rarely used in APIs, but web pages do this with JavaScript.

## References

*   [Architectural Styles and the Design of Network-based Software Architectures (Roy Thomas Fielding, 2000 Dissertation)](https://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm)
*   [MDN Web Docs Glossary: REST](https://developer.mozilla.org/en-US/docs/Glossary/REST)
*   [Amazon Web Services (AWS): What is a RESTful API?](https://aws.amazon.com/what-is/restful-api/)
