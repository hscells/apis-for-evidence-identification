# 2.2 Authentication and Rate limits

## Authentication and Authorisation

Authentication is the process of verifying the identity of a user. This is done by checking the user's credentials, such as a username and password, against a set of rules or policies. If the user's credentials are valid, they are granted access to the resource. If not, they are denied access.

Authorisation is the process of determining whether a user has the necessary permissions to access a resource. This is done by checking the user's credentials against a set of rules or policies. If the user has the necessary permissions, they are granted access to the resource. If not, they are denied access.

Some APIs require authentication to access their data. This is done to ensure that the data is only accessed by authorized users. There are several ways to authenticate with an API, including:

- API keys
- Basic authentication
- Token-based authentication
- JWT (JSON Web Token)

These details are not necessary for the workshop, but if you plan to work more with APIs in the future, it is good to know about these methods.

## Rate limits

Rate limiting is a way to control the number of requests that can be made to an API in a given time period. This is done to prevent abuse of the API and to ensure that all users have fair access to the data. The Entrez API, for example, has a rate limit of 3 requests per second. If you exceed this limit, you will receive an error message and your access may be restricted.

You can request an API key from NCBI to increase your rate limit. This will allow you to make more requests to the API in a given time period. Take a look at the [documentation](https://www.ncbi.nlm.nih.gov/books/NBK25497/#chapter2.API_Keys) for how to request and use an API key. For the purposes of this workshop, an API key is not required.

---
[top](../README.md#table-of-contents)<br/>
[previous: Data formats](2-1-data-formats.md)<br/>
[next: Using APIS via Python](2-4-using-apis-via-python.ipynb)<br/>