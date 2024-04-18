# 1.1 Conceptual introduction to APIs

An application programming interface (API) is a way for two or more computer programs or components to communicate with each other. An API is a software interface, offering a service to other pieces of software. A document or standard that describes how to build or use such a connection or interface is called an API specification. A computer system that meets this standard is said to implement or expose an API. The term API may refer either to the specification or to the implementation. Whereas a system's user interface specifies how end-users interact with the system, its API specifies how other programs interact with the system [[wikipedia](https://en.wikipedia.org/wiki/API)].

An API is like a waiter in a restaurant. The waiter takes your order, sends it to the kitchen, and then brings your food back to you. In this analogy, you are the customer, the kitchen is the server, and the waiter is the API. The API takes your request, sends it to the server, and then returns the server's response to you. The API acts as an intermediary between the client and the server, allowing them to communicate with each other [[freecodecamp](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)]. APIs all use a common language to communicate. This language is called HTTP (Hypertext Transfer Protocol). HTTP is the protocol used by the World Wide Web to define how messages are formatted and transmitted. It is the foundation of any data exchange on the Web [[freecodecamp](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)].

Basically, an API is a set of rules and protocols that allow different software applications to communicate with each other. APIs are used to define the methods and data formats that applications can use to request and exchange information. APIs are used in a wide range of applications, from web services to mobile apps. They are used to enable different software applications to communicate with each other and share data[[freecodecamp](https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/)].

For example, [NLM](https://www.nlm.nih.gov/) has an API that lets you search for articles across different databases like [PubMed](https://pubmed.ncbi.nlm.nih.gov/). Using the API of each database corresponds to what's known as an API endpoint. An API endpoint is a specific URL that represents an object or collection of objects. For example, the PubMed API has an endpoint that lets you search for articles by keyword. The endpoint for search is `https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi`. Endpoints are just URLs and you can even type these URLs into your browser! (https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi?db=pubmed&term=diagnostic&format=json). You can use this endpoint to search for articles by keyword, author, or publication date. We'll even see how in Sections [2.3](../2-how/2-3-using-apis-via-httpie.md) and [2.4](../2-how/2-4-using-apis-via-python.ipynb). The API returns the search results in a specific format, like JSON or XML which we'll learn more about in [Section 2.1](../2-how/2-1-data-formats.md). 

In summary, an API is a set of rules and protocols that allow different software applications to communicate with each other. APIs are used to define the methods and data formats that applications can use to request and exchange information. APIs are all accessed using URLs like you would type into your browser. When you access an API endpoint, you usually get back a response in a machine-readable format like JSON or XML.

## Making Requests

When you access an API, you are making a request to a server. The server then processes your request and sends back a response. There are several types of requests you can make to an API, including:

- `GET`: Retrieve data from the server
- `POST`: Send data to the server
- `PUT`: Update data on the server
- `DELETE`: Remove data from the server

We will only be using the `GET` request in this workshop.

## Online versus "Offline" APIs

APIs can be divided into two categories: online and "offline". Online APIs require an internet connection to access the data, while "offline" APIs do not. Online APIs are used to access data from a remote server, while "offline" APIs are used to access data stored locally on your computer. Online APIs are more common and are used to access data from web services like PubMed, ClinicalTrials.gov, and PubChem. "Offline" APIs are less common and are used to access data stored locally on your computer, like a database or a file.

"Offline" is in quotes since we normally just call these types of APIs "libraries". Libraries are collections of functions and routines that can be used to access data stored locally on your computer. There is an example of using an "offline" API in [Section 3.1](../3-use-cases/3-1-searching-pubmed.ipynb) where we replicate the experiments of [this paper](https://dl.acm.org/doi/pdf/10.1145/3539618.3591703) which used ChatGPT to formulate queries, but using our own local large language model.

--- 
[top](../README.md#table-of-contents)<br/>
[next: Limitations of APIs](1-2-limitations-of-apis.md)<br/>
