# JWT Decoder — Debug JSON Web Tokens Online

**Description:** Decode and inspect JSON Web Tokens (JWT) instantly. View header, payload, and signature. Client-side only, secure, and fast.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/jwt-decoder)**

## Definition
A JWT Decoder is a debugging tool for developers working with JSON Web Tokens (RFC 7519). JWTs are a compact, URL-safe means of representing claims to be transferred between two parties. They are widely used for authentication (logging in) and information exchange. A JWT consists of three parts: Header, Payload, and Signature. This tool decodes the Base64Url encoded strings to reveal the human-readable JSON content within the Header and Payload. It allows you to verify the token's structure, check expiration times (exp), issuer (iss), and custom claims without needing a backend server.

## Benefits
- Instant Debugging: Instantly visualize the Header and Payload of any JWT
- Expiration Check: Converts 'exp' and 'iat' timestamps to human-readable dates
- Secure: Tokens are decoded locally; your session data never hits our servers
- No Secret Required: Decodes payload without needing the private key or secret
- Structure Validation: Checks if the token follows the correct 3-part format
- Claim Inspection: Verify user roles, permissions, and issuer details
- Copy JSON: One-click copy for the decoded JSON payload
- Advanced & Safe: The most advanced safe JWT debugger for web developers

## Input Specifications
- JWT String (header.payload.signature)
- Bearer Token

## Output Specifications
- Decoded Header (JSON)
- Decoded Payload (JSON)
- Signature status (structure check only)

## Common Errors
- Pasting only the payload instead of the full token
- Confusing Decoding with Verifying (we don't check the signature validity against a secret)
- Using expired tokens

## Usage Scenarios
### Auth Debugging
Frontend developers checking if a user's token contains the correct roles or permissions.
**Keywords:** Auth0, Firebase Auth, User roles, Token debugging

### Session Expiry
Verifying the 'exp' (expiration) claim to understand why a user is being logged out.
**Keywords:** Token expiry, Session timeout, Unix timestamp

### API Integration
Backend developers inspecting tokens received from third-party providers to ensure correct claims.
**Keywords:** OIDC, OAuth2, Identity provider, Claims

## How To Use
1. Paste your JWT into the input area.
2. The tool automatically splits and decodes the Header and Payload.
3. Review the JSON output.
4. Hover over timestamp fields (iat, exp) to see human-readable dates.

## Example Input
```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c
```

## Example Output
```
Header: { "alg": "HS256", "typ": "JWT" }
Payload: { "sub": "1234567890", "name": "John Doe", "iat": 1516239022 }
```

## Code Samples
### JavaScript
```javascript
function parseJwt (token) {
    var base64Url = token.split('.')[1];
    var base64 = base64Url.replace(/-/g, '+').replace(/_/g, '/');
    var jsonPayload = decodeURIComponent(window.atob(base64).split('').map(function(c) {
        return '%' + ('00' + c.charCodeAt(0).toString(16)).slice(-2);
    }).join(''));

    return JSON.parse(jsonPayload);
}
```

## FAQ
### Is it safe to paste my JWT here?
Yes, 100%. I decode the token right here in your browser using JavaScript. It never leaves your device.

### Can I verify the signature?
I can decode the payload, but I don't verify the signature because that would require your secret key, which you should never share.

### Can I edit the JWT?
You can edit the JSON to see how it looks, but the token won't work on your server because the signature will be invalid.

### What algorithms are supported?
I support all of them! Since I'm just reading the Base64 structure, I can display any valid JWT regardless of the algorithm used.

## Related Tools
- base64
- hash-generator

