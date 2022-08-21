---
title: Request and Response Formats
layout: default 
---

# Error Handling

The AYJ Club Platform API uses the following error codes and statuses to indicate the success or failure of an API request. Generally, a `2xx` status code means success. A `4xx` status code usually means something is wrong with the parameters of the request, and a `5xx` status code means that there is something wrong with the AYJ Club Platform Server.

## Authentication

Errors that arise from authentication flows are documented in the [authentication]() documentation page, and contain a specific set of error types.

## Status Code Summary

| Code | Description | 
| --- | --- |
| 200 - OK | Everything worked as expected. |
| 201 - Created | Usually for POST requests, the resource was created successfully. |
| 400 - Bad Request | The request was unacceptable, usually because of a missing parameter or invalid header. |
| 401 - Unauthorized | The request was unacceptable because of invalid access token. |
| 403 - Forbidden | Your access level cannot unlock this endpoint. |
| 404 - Not Found | The resource you're looking for couldn't be found. |
| 409 - Conflict | Usually for POST requests, the resource you are trying to create already exists. |
| 429 - Too Many Requests | Too many requests hit the API too quickly. |
| 5xx - Server Error | For developers, please check the log to fix the server error. Something went wrong on the AYJ Club Platform Server. |


## Error Types

Each error given by the AYJ Club Platform API has a type attribute. This error type attribute can be handled automatically and you may refer to this table for a comprehensive description.

| Error | Description |
| --- | --- |
| 