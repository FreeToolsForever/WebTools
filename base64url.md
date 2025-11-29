# Base64URL Encoder & Decoder — URL Safe Base64

**Description:** Encode and decode Base64URL strings. URL-safe variant of Base64 (RFC 4648). Essential for JWTs and URL parameters.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/base64url)**

### Specific Tools
- 🔗 **[Base64URL Encoder](https://www.thefreewebtools.com/security-crypto/base64url/encoder)**: Encode to Base64URL.
- 🔗 **[Base64URL Decoder](https://www.thefreewebtools.com/security-crypto/base64url/decoder)**: Decode from Base64URL.

## Definition
Base64URL is a modification of the standard Base64 encoding scheme, designed to be safe for use in URLs and filenames. Standard Base64 uses characters '+' and '/', which have special meanings in URLs and file systems. Base64URL replaces '+' with '-' (minus) and '/' with '_' (underscore), and typically omits the padding '=' characters. This makes it ideal for encoding binary data (like digital signatures or tokens) that needs to be passed in URL query parameters without requiring percent-encoding. It is the standard encoding used for JSON Web Tokens (JWT).

## Benefits
- URL Safe: Replaces '+' and '/' with '-' and '_' for safe use in links
- JWT Standard: The required encoding format for JSON Web Tokens
- Filename Safe: Create safe filenames without reserved characters
- Privacy: 100% Client-side processing; secure and private
- Padding Handling: Automatically manages '=' padding for you
- Bidirectional: Convert between Standard Base64 and Base64URL
- Instant Conversion: See results immediately as you type
- Best & Fast: The best fast Base64URL converter for web developers

## Share Feature
Share Base64URL encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Base64URL strings
- Standard Base64 strings
- Plain text

## Output Specifications
- Base64URL string (no padding)
- Decoded text
- Copy-ready result

## Common Errors
- Confusing Base64 with Base64URL
- Expecting padding '=' (Base64URL often omits it)
- Decoding binary data as text (results in garbage)

## Usage Scenarios
### JWT Handling
Developers manually encoding or decoding parts of a JSON Web Token.
**Keywords:** JWT, Token encoding, JWS, JWE

### URL Parameters
Passing binary data or complex strings in URLs without breaking the link structure.
**Keywords:** Query param, Safe URL, Data transmission

### Filename Encoding
Encoding arbitrary data to be used as a safe filename.
**Keywords:** Safe filename, File system, Encoding

## How To Use
1. Paste your text or Base64URL string.
2. Select 'Encode' to convert to Base64URL.
3. Select 'Decode' to convert back to text.
4. Copy the result.

## Example Input
```
Hello World!
```

## Example Output
```
SGVsbG8gV29ybGQh
```

## Code Samples
### JavaScript
```javascript
function base64UrlEncode(str) {
  return btoa(str)
    .replace(/\+/g, '-')
    .replace(/\//g, '_')
    .replace(/=+$/, '');
}
```

## FAQ
### What is the difference between Base64 and Base64URL?
Base64 uses '+' and '/', which break URLs. Base64URL uses '-' and '_', which are safe for links and filenames.

### Why remove padding?
The '=' padding isn't URL-safe and takes up space. Base64URL usually removes it to be more compact.

### Can I use this for JWTs?
Yes! JWTs require Base64URL encoding. This tool is perfect for manually creating or editing JWT parts.

## Related Tools
- base64
- jwt-decoder

