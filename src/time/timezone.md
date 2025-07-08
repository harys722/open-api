---
label: Timezone Info
icon: clock
tags: [endpoint]
---

# Time Endpoint
The **Timezone Info** endpoint allows you to retrieve the details of the specified timezone. It can show the current time, unix timestamp, today's date with both gregorian and hijri.

## Endpoint
- **URL:** `https://api.harys.is-a.dev/v1/time`
- **Method:** `GET`
- **Description:** This endpoint shows the current time and other details of the specified timezone.

### URL Parameters
| Key  | Value |
| ------------- | ------------- |
| timezone  | The timezone you wish to get the info of: Between -1 & 14 |

### HTTP Header
| Key  | Value |
| ------------- | ------------- |
| Authorization  | Your own personal API key that you've requested. |

## Request Example
```
https://api.harys.is-a.dev/v1/time?timezone=1
```

### Response
```js
{
    "time": {
        "formatted": "05:10:55 PM",
        "unix": 1751821855,
        "UTC": "2025-07-06T16:10:56.034Z",
        "timezone": {
            "offset": 1,
            "name": "UTC",
            "region": "Berlin"
        }
    },
    "gregorian": {
        "date": "06-07-2025",
        "dayOfYear": 187,
        "weekNumber": 27,
        "humanReadable": "6 Jul, 2025"
    },
    "hijri": {
        "date": "11 Muḥarram 1447",
        "day": "11",
        "month": "Muḥarram",
        "year": "1447"
    },
    "docs": "https://open-api.js.org/",
    "github": "https://github.com/harys722/open-api"
}
```

> [!NOTE]
> The timezone parameter must be valid number between **-1** and **14**. The endpoint doesn't support EST, CET or PST, etc, text form timezones.
