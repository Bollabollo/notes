# The Request
Personal note: Maybe learn cURL
Good resource:
```
https://www.smashingmagazine.com/2018/01/understanding-using-rest-api/
```
## Endpoint
A URL requested by the user. It follows the structure below:
```
root-endpoint/?
```
### Root endpoint
The starting point of the API you are referring to. For example, Github's root endpoint is:
```
https://api.github.com
```

### Path
The resource being requested for - goes after the root endpoint

### Query Parameters
This is not part of the REST API but is often used. These always follow after the ```?``` and structured as a key-value pair separated by ampersand (```&```). Example:

![Query_string](https://github.com/Danglevuminh/notes/blob/master/img/Query_string.png)

Here, ```https://en.wikipedia.org/``` is the root endpoint; ```/w/index.php``` is the path; and ```?title=Query_string&action=edit.``` are the query parameters.

## Types of Request
```GET```: Get a resource from a server. Server finds the data then sends it back to user. This performs a ```READ``` operation.
```POST```: Creates a new resource on the server. Server creates new entry and tells user whether it is successful or not. This performs a ```CREATE``` operation.
```PUT```/```PATCH```: updates an entry in the database and tells user whether it is successful or not. This performs an ```UPDATE``` operation.
```DELETE```: deletes a resource from the server. Server deletes an entry from the database and tells user whether it is successful or not. This performs a ```DELETE``` operation.

# The Header

Provide information to both the client and the server. It can be used for authentication purposes and providing information about body content.

### HTTP Headers
**Property-value** pairs that are separated by a colon. The server expects JSON content from the header.
```
"Content-Type: application/json". Missing the opening "
```

### Data (or Body)
The data contains information you want to send to the server the option is only available with the types of request mentioned above.

### Authentication
There are two main ways to authenticate yourself: ```basic authentication using username and password``` and ```secret token (oauth2)```

# HTTPS status codes and error messages
**100+**: request being processed or provides information.
**200+**: request has **succeeded**
**300+**: request is directed to another URL
**400+**: an **error that originates from the client** has occurred
**500+**: an **error that originates from the server** has occurred

**HTTP status reference:**
```
https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
```

# API Request
A specific API version can be requested in two ways:
**Directly in the endpoint:** 
```
https://api.twitter.com/1.1/account/settings.json
```
**In a request header:**
```
curl https://api.github.com -H Accept:application/vnd.github.v3+json
```

