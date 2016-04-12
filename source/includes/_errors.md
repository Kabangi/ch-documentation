# Errors

COnnectHealth API uses the following error codes:


Error Code | Meaning
---------- | -------
422 | Bad Request -- Invalid request
401 | Unauthorized -- Your API key is wrong
403 | Forbidden -- Not authorized to access the requested  resource
404 | Not Found -- The specified resource could not be found
405 | Method Not Allowed -- You tried to access a resource with an invalid method
406 | Not Acceptable -- You requested unsupported format
410 | Gone -- The requested resource has been removed from our servers
429 | Too Many Requests -- You're requesting too many requests
500 | Internal Server Error -- We had a problem with our server. Try again later.
503 | Service Unavailable -- We're temporarially offline for maintanance. Please try again later.
