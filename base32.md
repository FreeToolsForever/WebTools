# Base32 Encoder & Decoder — RFC 4648 Standard

**Description:** Encode and decode Base32 strings. Case-insensitive encoding using A-Z and 2-7. Used in TOTP (Google Authenticator) and legacy systems.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/base32)**

### Specific Tools
- 🔗 **[Base32 Encoder](https://www.thefreewebtools.com/security-crypto/base32/encoder)**: Encode to Base32.
- 🔗 **[Base32 Decoder](https://www.thefreewebtools.com/security-crypto/base32/decoder)**: Decode from Base32.

## Definition
Base32 is a binary-to-text encoding scheme that uses a 32-character set, typically comprising the uppercase letters A-Z and the digits 2-7. It is defined in RFC 4648. Base32 is less efficient than Base64 (taking up more space) but has the advantage of being case-insensitive and avoiding visually ambiguous characters (like 'I', 'l', '1', '0', 'O'). This makes it ideal for human usage, such as typing product keys or verification codes manually. It is notably used in the generation of TOTP secrets for Two-Factor Authentication apps like Google Authenticator.

## Benefits
- Human Readable: Case-insensitive encoding reduces transcription errors
- TOTP Standard: The format used for Google Authenticator 2FA secrets
- Ambiguity Free: Avoids confusing characters like '1', 'l', '0', 'O'
- Privacy: 100% Client-side processing
- Legacy Support: Compatible with older systems requiring case-insensitive input
- Bidirectional: Encode and Decode with a single click
- RFC 4648: Follows the standard specification strictly
- Best & Secure: The best secure Base32 tool for 2FA keys

## Share Feature
Share Base32 encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Plain text
- Base32 strings
- Binary data

## Output Specifications
- Base32 string
- Decoded text
- Copy-ready result

## Common Errors
- Using '0', '1', or '8' (not in Base32 alphabet)
- Confusing with Base64
- Case sensitivity expectations (it's case-insensitive)

## Usage Scenarios
### Two-Factor Auth
Encoding the secret key for Google Authenticator or Authy (which use Base32).
**Keywords:** TOTP, 2FA, Google Authenticator, Secret key

### Product Keys
Generating license keys that are easy for users to type without confusion.
**Keywords:** License key, Product code, Serial number

### File Systems
Encoding filenames in case-insensitive file systems where Base64 might cause collisions.
**Keywords:** Filename encoding, Case insensitive, Legacy system

## How To Use
1. Paste your text or Base32 string.
2. Select 'Encode' to convert to Base32.
3. Select 'Decode' to convert back to text.
4. Copy the result.

## Example Input
```
Hello
```

## Example Output
```
JBSWY3DP
```

## Code Samples
### Python
```python
import base64
encoded = base64.b32encode(b'Hello')
print(encoded)
```

## FAQ
### Why use Base32 instead of Base64?
Base32 is case-insensitive and avoids confusing letters like 'I' and 'l'. It's much better for codes that humans have to type manually.

### What characters are used?
I use A-Z and 2-7. I skip '0', '1', and '8' so you don't confuse them with 'O', 'I', or 'B'.

### Is it secure?
No, it's just encoding. It makes data safe to transport, but it doesn't hide the information from someone who wants to decode it.

## Related Tools
- base64
- hex

