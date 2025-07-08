---
order: 1800
label: Decode String
icon: code
tags: [endpoint]
---

# Base64 Decode
The **Base64 Decode** endpoint enables you to effortlessly convert a Base64-encoded string back to its original text or data. Perfect for reversing Base64 encoding and extracting the original information from encoded inputs.

## Endpoint
- **URL:** `https://api.harys.is-a.dev/v1/base64/decode`
- **Method:** `POST`
- **Description:** This endpoint decodes the base64-encoded string to its original text or data.

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
https://api.harys.is-a.dev/v1/base64/decode

{
  "string": "T3BlbiBBUEk="
}
```

### Response
```js
{
    "base64": {
        "string": "T3BlbiBBUEk=",
        "decoded": "Open API"
    },
    "info": {
        "docs": "https://open-api.js.org/",
        "github": "https://github.com/harys722/open-api"
    }
}
```
