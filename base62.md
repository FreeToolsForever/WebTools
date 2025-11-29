# Base62 Encoder & Decoder — URL Shortener Format

**Description:** Encode and decode Base62 strings. Uses 0-9, A-Z, a-z. High-density encoding for URL shorteners and unique IDs.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/base62)**

### Specific Tools
- 🔗 **[Base62 Encoder](https://www.thefreewebtools.com/security-crypto/base62/encoder)**: Encode to Base62.
- 🔗 **[Base62 Decoder](https://www.thefreewebtools.com/security-crypto/base62/decoder)**: Decode from Base62.

## Definition
Base62 is a positional numeral system that uses 62 characters: 0-9, A-Z, and a-z. It is essentially Base64 without the special characters '+' and '/' (and usually without padding). This makes it extremely popular for URL shortening services (like YouTube's youtu.be links) because the resulting strings are URL-safe, compact, and do not contain any non-alphanumeric characters that might be stripped or modified by some systems. Unlike Base36, Base62 is case-sensitive, allowing it to store more information in fewer characters.

## Benefits
- High Density: Stores more data per character than Base36 or Hex
- URL Safe: Contains only alphanumeric characters; no special symbols
- Case Sensitive: Distinguishes between 'A' and 'a' for maximum efficiency
- Privacy: 100% Client-side processing
- Shortener Standard: The de-facto standard for modern URL shorteners
- Bidirectional: Encode and Decode instantly
- Clean Output: No padding or special characters
- Best & Compact: The best compact Base62 tool for developers

## Share Feature
Share Base62 encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Integers (for conversion)
- Plain text
- Base62 strings

## Output Specifications
- Base62 string
- Decoded integer/text
- Copy-ready result

## Common Errors
- Assuming case-insensitivity (Base62 is case-sensitive)
- Confusing with Base64 (Base62 has no + or /)
- Using symbols (only 0-9, A-Z, a-z allowed)

## Usage Scenarios
### URL Shorteners
Creating the shortest possible URL slugs (e.g., bit.ly/3hQ2vP).
**Keywords:** Short link, TinyURL, Slug, Link compression

### Unique IDs
Generating compact, unique identifiers for database records exposed in URLs.
**Keywords:** Public ID, Resource ID, Compact ID

### Obfuscation
Hiding sequential database IDs (like 1, 2, 3) by converting them to random-looking Base62 strings.
**Keywords:** ID masking, Obfuscation, Security through obscurity

## How To Use
1. Paste your text or number.
2. Select 'Encode' to convert to Base62.
3. Select 'Decode' to convert back.
4. Copy the result.

## Example Input
```
Hello World
```

## Example Output
```
73XpUgyMwkGr
```

## Code Samples
### JavaScript (base62)
```javascript
const base62 = require('base62');
const encoded = base62.encode(12345);
console.log(encoded); // '3D7'
```

## FAQ
### Why Base62 instead of Base64?
Base62 is safer for URLs because it doesn't use '+' or '/'. It's slightly less efficient but guarantees no broken links.

### Is it case sensitive?
Yes! 'A' and 'a' are different. This allows me to pack more data into a shorter string compared to Base36.

### Can I encode negative numbers?
Standard Base62 is for positive integers. If you need to encode negative numbers, I usually treat them as unsigned or add a sign prefix.

## Related Tools
- base36
- base58

