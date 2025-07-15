---
label: QOTD
icon: question
tags: [endpoint]
---

# QOTD - Question of the Day
The Question of the Day (QOTD) endpoint provides a new, interesting random question, which can be used as daily event to engage users and promote daily interaction.

## Endpoint
- **URL:** `https://api.harys.is-a.dev/v1/qotd`
- **Method:** `GET`
- **Description:** This endpoint provides a random question.

### URL Parameters
| Key  | Value |
| ------------- | ------------- |
| count  | The count of questions you wish to get. |

> [!NOTE]
> You can only set it to 5, if it is long then only 5 questions will be returned.

### HTTP Header
| Key  | Value |
| ------------- | ------------- |
| Authorization  | Your own personal API key that you've requested. |

## Request Example
```
https://api.harys.is-a.dev/v1/qotd
```

```json Response
{
    "questions": ["How do you practice self-care?"],
    "total_questions": 220,
    "requested_count": 1,
    "info": {
        "docs": "https://open-api.js.org/",
        "github": "https://github.com/harys722/open-api"
    }
}
```
