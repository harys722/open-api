---
order: 1800
label: Number Analyzer
icon: number
tags: [endpoint]
---

# Number Analyzer
The **Number Analyzer** endpoint provides a comprehensive analysis of any given number or random number. It evaluates various properties and characteristics, including whether the number is positive or negative, even or odd, prime, a Fibonacci number, a perfect square, an Armstrong number, or a palindrome. Additionally, it calculates divisibility by common numbers like 3, 5, and 10, provides modulo results, counts the digits, and identifies prime factors. This tool offers detailed insights into the nature of any number you input, making it useful for mathematical exploration and validation.

## Endpoint
- **URL:** `https://api.harys.is-a.dev/v1/math/number-analyzer`
- **Method:** `GET`
- **Description:** This endpoint provides a comprehensive analysis of any given number or random number.

### URL Parameters
| Key  | Value |
| ------------- | ------------- |
| number  | The number you would like to get the analysis of. |
| min  | Specify the minimum number to retrieve the random number. |
| max  | Specify the maximum number to retrieve the random number. |

> [!NOTE]
> If you don't provide the `number` parameter, it will grab the random number between 1 and 10,000.

### HTTP Header
| Key  | Value |
| ------------- | ------------- |
| Authorization  | Your own personal API key that you've requested. |

## Request Example
```
https://api.harys.is-a.dev/v1/math/number-analyzer?number=999
```

### Response
```js
{
    "number": 999,
    "absoluteValue": 999,
    "isNegative": false,
    "isGreaterThanZero": true,
    "isEven": false,
    "isOdd": true,
    "isDecimal": false,
    "isPrime": false,
    "isFibonacci": false,
    "isPerfectSquare": false,
    "isArmstrong": false,
    "isPalindrome": true,
    "isDivisibleBy3": true,
    "isDivisibleBy5": false,
    "isDivisibleBy10": false,
    "modulo3": 0,
    "modulo5": 4,
    "modulo7": 5,
    "digitCount": 3,
    "primeFactors": [3, 3, 3, 37],
    "formatted1": "999",
    "formatted2": "999",
    "abbreviated": "999",
    "numberType": "integer",
    "info": {
        "docs": "https://open-api.js.org/",
        "github": "https://github.com/harys722/open-api"
    }
}
```