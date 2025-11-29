# HMAC Generator — Hash-based Message Authentication Code

**Description:** Generate HMAC using SHA256, SHA512, MD5, and more. Securely sign messages with a secret key.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/hmac-generator)**

## Definition
HMAC (Hash-based Message Authentication Code) is a specific type of message authentication code (MAC) involving a cryptographic hash function and a secret cryptographic key. It may be used to simultaneously verify both the data integrity and the authentication of a message.

## Benefits
- Security: Verifies both integrity and authenticity
- Versatile: Supports multiple hash algorithms
- Privacy: 100% Client-side processing
- Standard: Compliant with RFC 2104

## Share Feature
Share generated HMAC. (Limit: 1KB)

## Input Specifications
- Message text
- Secret key
- Algorithm selection

## Output Specifications
- HMAC string

## Common Errors
- Using weak keys
- Mismatched algorithms

## Usage Scenarios
### API Authentication
Signing API requests to verify sender identity.
**Keywords:** API signature, Request signing

## How To Use
1. Enter your message.
2. Enter your secret key.
3. Select the hash algorithm.
4. Copy the generated HMAC.

## Example Input
```
Message: Hello, Key: Secret
```

## Example Output
```
HMAC-SHA256: ...
```

## Code Samples
### Node.js
```node.js
const crypto = require('crypto');
const hmac = crypto.createHmac('sha256', 'Secret');
hmac.update('Hello');
console.log(hmac.digest('hex'));
```

## FAQ
### Is the key sent to the server?
No, everything is processed locally in your browser.

## Related Tools
- hash-generator

