# Base91 Encoder & Decoder — High Efficiency Encoding

**Description:** Encode and decode Base91 strings. Extremely efficient binary-to-text encoding. Smaller than Base64 and Ascii85.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/base91)**

### Specific Tools
- 🔗 **[Base91 Encoder](https://www.thefreewebtools.com/security-crypto/base91/encoder)**: Encode to Base91.
- 🔗 **[Base91 Decoder](https://www.thefreewebtools.com/security-crypto/base91/decoder)**: Decode from Base91.

## Definition
basE91 is an advanced method for encoding binary data as ASCII text. It is similar to Base64 but is significantly more efficient. The overhead produced by basE91 depends on the input data but amounts to at most 23% (compared to 33% for Base64 and 25% for Ascii85). It uses 91 printable ASCII characters. This makes it one of the most space-efficient binary-to-text encoding schemes available, ideal for transmitting large amounts of data over text-based protocols.

## Benefits
- Maximum Efficiency: Lowest overhead (~23%) of common encodings
- High Density: Packs more data into fewer characters
- Privacy: 100% Client-side processing
- Bidirectional: Encode and Decode instantly
- Flexible: No padding characters required
- Text Safe: Uses printable ASCII characters
- Fast Processing: Optimized for speed in the browser
- Best & Compact: The best high-efficiency encoding tool

## Share Feature
Share Base91 encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Plain text
- Base91 strings
- Binary data

## Output Specifications
- Base91 string
- Decoded text
- Copy-ready result

## Common Errors
- Using characters outside the Base91 alphabet
- Expecting standard padding (Base91 doesn't use it)
- Compatibility issues (less common than Base64)

## Usage Scenarios
### Bandwidth Optimization
Transmitting large binary payloads over JSON or XML where size matters.
**Keywords:** Data compression, Payload size, Optimization

### Email Attachments
Sending files via email with less overhead than standard Base64 encoding.
**Keywords:** Email size, Attachment encoding, MIME alternative

### Database Storage
Storing binary blobs in text fields with minimal wasted space.
**Keywords:** Blob storage, Text field, Database optimization

## How To Use
1. Paste your text or Base91 string.
2. Select 'Encode' to convert to Base91.
3. Select 'Decode' to convert back.
4. Copy the result.

## Example Input
```
Hello World
```

## Example Output
```
>OwJh>Io0Tv
```

## Code Samples
### C
```c
// basE91 C library usage
struct basE91 b91;
basE91_init(&b91);
basE91_encode(&b91, input, len, output);
```

## FAQ
### Why is it called Base91?
Because it uses 91 different characters from the ASCII table to represent data.

### Is it better than Base64?
For size? Yes, definitely. It produces smaller strings. For compatibility? No, Base64 is supported everywhere; Base91 is more niche.

### Can I use it in URLs?
Not directly. It uses characters like double quotes and backslashes that need to be escaped in URLs.

## Related Tools
- base64
- ascii85

