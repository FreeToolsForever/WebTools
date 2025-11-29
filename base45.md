# Base45 Encoder & Decoder — QR Code Standard

**Description:** Encode and decode Base45 strings. The standard encoding for QR codes and EU Digital COVID Certificates. Optimized for alphanumeric mode.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/base45)**

### Specific Tools
- 🔗 **[Base45 Encoder](https://www.thefreewebtools.com/security-crypto/base45/encoder)**: Encode to Base45.
- 🔗 **[Base45 Decoder](https://www.thefreewebtools.com/security-crypto/base45/decoder)**: Decode from Base45.

## Definition
Base45 is a binary-to-text encoding scheme defined in RFC 9285. It is specifically designed to be used in QR codes. QR codes have an 'alphanumeric' mode that can store 45 specific characters (0-9, A-Z, space, $, %, *, +, -, ., /, :) more efficiently than general binary data. Base45 encodes any binary data into this 45-character set, allowing QR codes to store significantly more data in the same space compared to Base64. It is famously used in the EU Digital COVID Certificate (Green Pass).

## Benefits
- QR Optimized: Maximizes data density in QR codes
- EU Standard: The encoding used for EU Digital COVID Certificates
- High Efficiency: Stores more data in a QR code than Base64
- Privacy: 100% Client-side processing
- RFC 9285: Follows the official IETF specification
- Bidirectional: Encode and Decode instantly
- Specialized: The only tool you need for decoding Green Pass raw data
- Best & Niche: The best specialized Base45 tool for QR developers

## Share Feature
Share Base45 encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Plain text
- Base45 strings
- Binary data

## Output Specifications
- Base45 string
- Decoded text
- Copy-ready result

## Common Errors
- Using characters outside the 45 allowed chars
- Confusing with Base64 or Base32
- Expecting it to work efficiently outside of QR codes

## Usage Scenarios
### QR Code Generation
Encoding binary data (like compressed CWTs) to fit into a smaller QR code.
**Keywords:** QR code capacity, Alphanumeric mode, Data density

### Health Certificates
Decoding the raw payload of an EU Digital COVID Certificate.
**Keywords:** Green Pass, COVID certificate, HC1, Health data

### Compact Storage
Storing binary data on printed media where alphanumeric characters are preferred.
**Keywords:** Printed code, Optical storage, Paper backup

## How To Use
1. Paste your text or Base45 string.
2. Select 'Encode' to convert to Base45.
3. Select 'Decode' to convert back.
4. Copy the result.

## Example Input
```
Hello World
```

## Example Output
```
%69 VD92EX0
```

## Code Samples
### Python
```python
import base45
encoded = base45.b45encode(b'Hello World')
print(encoded)
```

## FAQ
### Why Base45?
QR codes have a special mode for 45 specific characters. Base45 converts data to use exactly those characters, making the QR code smaller.

### What characters are used?
I use 45 specific characters: 0-9, A-Z, space, $, %, *, +, -, ., /, and :.

### Is it widely used?
Yes! It's the standard for things like the EU Digital COVID Certificate and other modern QR-based systems.

## Related Tools
- qr-code-generator
- base64

