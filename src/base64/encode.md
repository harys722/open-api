---
order: 2000
label: Encode String
icon: code
tags: [endpoint]
---

# Base64 Decode
The Base64 Encode endpoint converts an input string or data into Base64 format, which encodes binary data into a text-based representation.

## Endpoint
- **URL:** `https://api.harys.is-a.dev/v1/base64/encode`
- **Method:** `POST`
- **Description:** The Base64 Encode endpoint converts a string to Base64 format.

### Request Body
| Key  | Value |
| ------------- | ------------- |
| string  | The base64-encoded string you would like to decode. |

### HTTP Header
| Key  | Value |
| ------------- | ------------- |
| Authorization  | Your own personal API key that you've requested. |

## Request Example
```js
https://api.harys.is-a.dev/v1/base64/encode

{
  "string": "Open API"
}
```

### Response
```js
{
    "base64": {
        "string": "Open API",
        "encoded": "T3BlbiBBUEk="
    },
    "info": {
        "docs": "https://open-api.js.org/",
        "github": "https://github.com/harys722/open-api"
    }
}
```
