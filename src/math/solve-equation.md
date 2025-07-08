---
order: 2000
label: Solve Equation
icon: diff-added
tags: [endpoint]
---

# Solve Equation
Easily solve mathematical expressions with our **Solve Equation** endpoint. Whether it's simple addition like 2 + 2 or more complex trail equations such as 1 + 1 + 1 + 1, this tool handles them all seamlessly.

## Endpoint
- **URL:** `https://api.harys.is-a.dev/v1/math/solve-equation`
- **Method:** `GET`
- **Description:** This endpoint can help you solve the math equations.

### URL Parameters
| Key  | Value |
| ------------- | ------------- |
| equation  | The equation you wish to calculate. |

### HTTP Header
| Key  | Value |
| ------------- | ------------- |
| Authorization  | Your own personal API key that you've requested. |

## Request Example
```
https://api.harys.is-a.dev/v1/math/solve-equation?equation=(12*100)/500
```

### Response
```js
{
    "equation": "(12*100)/500",
    "result": 2.4,
    "success": true,
    "info": {
        "docs": "https://open-api.js.org/",
        "github": "https://github.com/harys722/open-api"
    }
}
```

> [!NOTE]
> The equation parameter can support complex equations included ( ) brackets.
