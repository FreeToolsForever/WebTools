# Base36 Encoder & Decoder — Alphanumeric Converter

**Description:** Convert numbers and text to Base36. Uses 0-9 and A-Z. Compact case-insensitive encoding for URL shorteners and IDs.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/base36)**

### Specific Tools
- 🔗 **[Base36 Encoder](https://www.thefreewebtools.com/security-crypto/base36/encoder)**: Encode to Base36.
- 🔗 **[Base36 Decoder](https://www.thefreewebtools.com/security-crypto/base36/decoder)**: Decode from Base36.

## Definition
Base36 is a positional numeral system that uses 36 symbols: the Arabic numerals 0–9 and the Latin letters A–Z. It is the most compact case-insensitive alphanumeric numeral system. This property makes it extremely useful for creating human-readable identifiers that need to be communicated verbally or typed manually without worrying about capitalization. It is widely used in URL shortening services (like bit.ly), product serial numbers, and legacy systems that do not support case sensitivity.

## Benefits
- Case Insensitive: 'A' and 'a' are treated as the same value
- Compact: Represents large numbers in fewer characters than decimal
- URL Friendly: Safe for use in URLs without encoding
- Privacy: 100% Client-side processing
- Legacy Compatible: Works with systems that uppercase all input
- Bidirectional: Encode and Decode instantly
- Simple Alphabet: Uses only 0-9 and A-Z
- Best & Simple: The best simple Base36 converter for developers

## Share Feature
Share Base36 encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Integers (for conversion)
- Plain text
- Base36 strings

## Output Specifications
- Base36 string
- Decoded integer/text
- Copy-ready result

## Common Errors
- Using special characters (only 0-9 and A-Z allowed)
- Expecting case sensitivity
- Confusing with Base62 (which is case-sensitive)

## Usage Scenarios
### URL Shortening
Converting database IDs (integers) to short alphanumeric strings for links.
**Keywords:** URL shortener, Slug generation, Short link

### Asset Tagging
Creating compact, case-insensitive serial numbers for physical inventory.
**Keywords:** Asset tag, Serial number, Inventory ID

### Legacy Systems
Interfacing with old mainframes or file systems that only support uppercase alphanumeric characters.
**Keywords:** Mainframe, Legacy support, Uppercase only

## How To Use
1. Paste your text or number.
2. Select 'Encode' to convert to Base36.
3. Select 'Decode' to convert back.
4. Copy the result.

## Example Input
```
123456789
```

## Example Output
```
21I3V9
```

## Code Samples
### JavaScript
```javascript
const num = 123456789;
const base36 = num.toString(36).toUpperCase();
console.log(base36);
```

### Python
```python
def base36encode(number):
    alphabet = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ'
    base36 = ''
    while number:
        number, i = divmod(number, 36)
        base36 = alphabet[i] + base36
    return base36 or alphabet[0]
```

## FAQ
### Why Base36?
It's the most efficient way to store data using only numbers and letters without worrying about capitalization.

### What is the largest Base36 number?
Technically infinite, but in JavaScript, the safe integer limit applies. I handle large numbers as strings to avoid errors.

### Can I use special characters?
No. Base36 only supports 0-9 and A-Z. Any other character will cause an error.

## Related Tools
- base62
- hex

