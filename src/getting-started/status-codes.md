---
order: 1800
label: Status Codes
icon: rss
permalink: /status-codes
nav:
  badge: NEW|info
tags: [info]
---

# Status Codes
When interacting with APIs, various HTTP status codes are returned to indicate the outcome of the request. Each code provides specific information about the response. Below is a detailed list of common HTTP status codes can be return by our API service.

---

## 200: OK

**Description:**  
The request was successful, and the server responded with the requested data. This is the standard response for successful HTTP requests.

**When to expect:**  
Whenever an API call is handled correctly and returns the expected result. For example, a successful GET, POST, PUT, or DELETE request will typically return 200 OK (though POST may also return 201 Created).

---

## 400: Bad Request

**Description:**  
The server could not understand the request due to invalid syntax. This often means there is something wrong with the request body, parameters, or query string.

**When to expect:**  
If required fields are missing, JSON formatting is incorrect, or data types do not match the API specification.

---

## 401: Unauthorized

**Description:**  
Authentication is required and has either not been provided or failed. The client must authenticate itself to get the requested response.

**When to expect:**  
When API requests are made without a valid authentication token or with invalid credentials.

---

## 403: Forbidden

**Description:**  
The client is authenticated but does not have permission to access the requested resource. Authorization will not help, and the request should not be repeated.

**When to expect:**  
When a user tries to access a resource or perform an action they do not have rights for.

---

## 404: Not Found

**Description:**  
The requested resource could not be found on the server. This can happen if the endpoint URL is incorrect or the resource does not exist.

**When to expect:**  
When requesting a specific resource that does not exist, or using a wrong API endpoint.

---

## 405: Method Not Allowed

**Description:**  
The method specified in the request is not allowed for the resource. For example, trying to use POST on a resource that only supports GET.

**When to expect:**  
If you try to use an unsupported HTTP method for an endpoint.

---

## 429: Too Many Requests

**Description:**  
The user has sent too many requests in a given amount of time ("rate limiting"). The response may include information about how long to wait before making a new request.

**When to expect:**  
If you exceed the API's rate limits.

---

## 500: Internal Server Error

**Description:**  
An unexpected condition was encountered by the server. This is a generic error message indicating the server failed to fulfill a valid request.

**When to expect:**  
When something goes wrong on the server side, often unrelated to the request.

---

## 502: Bad Gateway

**Description:**  
The server was acting as a gateway or proxy and received an invalid response from the upstream server.

**When to expect:**  
If the API relies on other services that are currently failing.

---

## 503: Service Unavailable

**Description:**  
The server is currently unable to handle the request due to temporary overload or scheduled maintenance.

**When to expect:**  
During server maintenance or temporary overloading.

---

## 504: Gateway Timeout

**Description:**  
The server was acting as a gateway or proxy and did not receive a timely response from the upstream server.

**When to expect:**  
If the API takes too long to get a response from another service it depends on.
