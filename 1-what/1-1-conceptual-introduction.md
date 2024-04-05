# 1.1 Conceptual introduction to APIs

An application programming interface (API) is a way for two or more computer programs or components to communicate with each other. It is a type of software interface, offering a service to other pieces of software. A document or standard that describes how to build or use such a connection or interface is called an API specification. A computer system that meets this standard is said to implement or expose an API. The term API may refer either to the specification or to the implementation. Whereas a system's user interface dictates how its end-users interact with the system in question, its API dictates how to write code that takes advantage of that system's capabilities [[wikipedia](https://en.wikipedia.org/wiki/API)].

An API is like a waiter in a restaurant. The waiter takes your order, sends it to the kitchen, and then brings your food back to you. In this analogy, you are the client, the kitchen is the server, and the waiter is the API. The API takes your request, sends it to the server, and then returns the server's response to you. The API acts as an intermediary between the client and the server, allowing them to communicate with each other [[freecodecamp](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)]. APIs all use a common language to communicate. This language is called HTTP (Hypertext Transfer Protocol). HTTP is the protocol used by the World Wide Web to define how messages are formatted and transmitted. It is the foundation of any data exchange on the Web [[freecodecamp](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)].

Basically, an API is a set of rules and protocols that allow different software applications to communicate with each other. APIs are used to define the methods and data formats that applications can use to request and exchange information. APIs are used in a wide range of applications, from web services to mobile apps. They are used to enable different software applications to communicate with each other and share data. APIs are used to define the methods and data formats that applications can use to request and exchange information. APIs are used in a wide range of applications, from web services to mobile apps. They are used to enable different software applications to communicate with each other and share data [[freecodecamp](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)].

For example, NLM has an API that lets you search for articles across different databases, like PubMed, ClinicalTrials.gov, and PubChem. Using the API of each database corresponds to what's known as an API endpoint. An API endpoint is a specific URL that represents an object or collection of objects. For example, the PubMed API has an endpoint that lets you search for articles by keyword. The endpoint for this search is `https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi`. Endpoints are just URLs and you can even type these URLs into your browser! (https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi?db=pubmed&term=diagnostic&format=json). You can use this endpoint to search for articles by keyword, author, or publication date. We'll even see how in Sections [2.3](../2-how/2-3-using-apis-via-httpie.md) and [2.4](../2-how/2-4-using-apis-via-python.ipynb). The API returns the search results in a specific format, like JSON or XML which we'll learn more about in Section [2.1](../2-how/2-1-data-formats.md). 

In summary, an API is a set of rules and protocols that allow different software applications to communicate with each other. APIs are used to define the methods and data formats that applications can use to request and exchange information. APIs are all accessed using URLs like you would type into your browser. When you access an API endpoint, you usually get back a response in a machine-readable format like JSON or XML.

## Making Requests

When you access an API, you are making a request to a server. The server then processes your request and sends back a response. There are several types of requests you can make to an API, including:

- `GET`: Retrieve data from the server
- `POST`: Send data to the server
- `PUT`: Update data on the server
- `DELETE`: Remove data from the server

--- 
[top](../README.md)<br/>
[next: Limitations of APIs](1-2-limitations-of-apis.md)<br/>