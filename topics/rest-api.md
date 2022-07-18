# The Request
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
