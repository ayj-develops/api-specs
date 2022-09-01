---
title: Errors
layout: default 
---

# Error Handling

The AYJ Club Platform API uses the following error codes and statuses to indicate the success or failure of an API request. Generally, a `2xx` status code means success. A `4xx` status code usually means something is wrong with the parameters of the request, and a `5xx` status code means that there is something wrong with the AYJ Club Platform Server.

## Authentication

Errors that arise from authentication flows are documented in the [authentication]({% link _docs/authentication.md %}) documentation page, and contain a specific set of error types.

## Status Code Summary

| Code                    | Description                                                                                                         |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------- |
| 200 - OK                | Everything worked as expected.                                                                                      |
| 201 - Created           | Usually for POST requests, the resource was created successfully.                                                   |
| 400 - Bad Request       | The request was unacceptable, usually because of a missing parameter or invalid header.                             |
| 401 - Unauthorized      | The request was unacceptable because of invalid access token.                                                       |
| 403 - Forbidden         | Your access level cannot unlock this endpoint.                                                                      |
| 404 - Not Found         | The resource you're looking for couldn't be found.                                                                  |
| 409 - Conflict          | Usually for POST requests, the resource you are trying to create already exists.                                    |
| 429 - Too Many Requests | Too many requests hit the API too quickly.                                                                          |
| 5xx - Server Error      | For developers, please check the log to fix the server error. Something went wrong on the AYJ Club Platform Server. |


## Error Types

Each error given by the AYJ Club Platform API has a type attribute. This error type attribute can be handled automatically and you may refer to this table for a comprehensive description.

| Error                 | Code | Description                                                                   |
| --------------------- | ---- | ----------------------------------------------------------------------------- |
| bad_parameter         | 400  | An invalid parameter was passed, either missing or incorrect value            |
| exceeded_char         | 400  | Character limit exceeded, usually happens on POST or PUT requests             |
| access_token_required | 401  | Missing a Bearer token from Firebase in the header of the request             |
| invalid_access_token  | 400  | An invalid Bearer token from Firebase was passed in the header of the request |
| access_denied         | 403  | The client's request does not meet the permission level required              |
| parameter_taken       | 409  | The resource field already exists                                             |
| not_found             | 404  | The resource doesn't exist or it can't be accessed by the server              |
| too_many_requests     | 429  | Too many requests                                                             |
| server_error          | 500  | Something went wrong with the server                                          |

Please refer to the [response formats]({% link _docs/formats.md %}) to see an example of an error response.