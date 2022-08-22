---
title: Request and Response Formats
layout: default 
---

## Common Object

All responses in the API share a common response object format, for consistency both on the developer end and on the client. 

Specific fields are added on top of the common response object for certain endpoints. While they differ, endpoint specific response objects still contain the required common object fields and may contain the optional common object fields.

### Fields

|             |                                                                                                                          |
| ----------- | ------------------------------------------------------------------------------------------------------------------------ |
| ok          | boolean, indicates success or failure                                                                                    |
| error_id    | integer, refers to [status code]({{ site.baseurl }}/docs/errors )<br>[may be optional]({{ site.baseurl }}/docs/optional) |
| error_name  | string<br>[may be optional]({{ site.baseurl }}/docs/optional)                                                            |
| description | string<br>[may be optional]({{ site.baseurl }}/docs/optional)                                                            |

### Example

```json
{
  "ok": true,
  "stuff": "some data from the API"
}
```

Refer to [error object example](#example-1) to view the common object response if something goes wrong.

## Error Object

This is a typical error response object that is returned when something goes wrong.

Please note that the `description` field is different than the `error_message` field on the common object responses. `description` provides extra commentary on the error type, while `error_message` is a direct stacktrace of the error.

### Fields

|             |                                    |
| ----------- | ---------------------------------- |
| description | string                             |
| error_id    | integer, refers to [status code]() |
| error_name  | string                             |

### Example

**Exceeded Character Limit**

```json
{
  "ok": false,
  "error_id": 400,
  "error_name": "exceeded_char",
  "description": "500 Character limit exceeded for new post body",
}
```
