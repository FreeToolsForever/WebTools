# Ascii85 (Base85) Encoder & Decoder — Adobe PDF Standard

**Description:** Encode and decode Ascii85 (Base85) strings. More efficient than Base64. Used in PDF and PostScript. Free online converter.

🚀 **[Try This Tool Online](https://www.thefreewebtools.com/security-crypto/ascii85)**

### Specific Tools
- 🔗 **[Ascii85 Encoder](https://www.thefreewebtools.com/security-crypto/ascii85/encoder)**: Encode to Ascii85.
- 🔗 **[Ascii85 Decoder](https://www.thefreewebtools.com/security-crypto/ascii85/decoder)**: Decode from Ascii85.

## Definition
Ascii85, also called Base85, is a form of binary-to-text encoding developed by Paul E. Rutter for the btoa utility. It is more efficient than Base64, expanding the data size by only 25% (compared to Base64's 33%). It uses 85 ASCII characters: '!' through 'u'. Ascii85 is widely known for its use in the PostScript and PDF file formats to embed binary data. It supports compression features like replacing four spaces with 'y' and four null bytes with 'z'.

## Benefits
- High Efficiency: 25% overhead vs 33% for Base64
- PDF Standard: The native encoding used inside PDF files
- Compression: Supports 'z' (nulls) and 'y' (spaces) shorthand
- Privacy: 100% Client-side processing
- Bidirectional: Encode and Decode instantly
- Adobe Compatible: Fully compatible with Adobe's implementation
- Large Data: Efficient for larger binary blobs
- Best & Efficient: The best efficient Ascii85 tool for PDF developers

## Share Feature
Share Ascii85 encoded/decoded strings. (Limit: 5KB)

## Input Specifications
- Plain text
- Ascii85 strings (<~...~>)
- Binary data

## Output Specifications
- Ascii85 string
- Decoded text
- Copy-ready result

## Common Errors
- Missing <~ and ~> delimiters (Adobe format requires them)
- Invalid characters (outside ! to u range)
- Confusing 'z' and 'y' exceptions

## Usage Scenarios
### PDF Analysis
Decoding binary streams extracted from PDF files to view their content.
**Keywords:** PDF stream, PostScript, Adobe, Binary embedding

### Data Compression
Encoding data for transmission where bandwidth is tighter than Base64 allows.
**Keywords:** Efficient encoding, Bandwidth saving, Data transfer

### Steganography
Hiding data in plain text using non-obvious encoding.
**Keywords:** Hidden data, Obfuscation, Text hiding

## How To Use
1. Paste your text or Ascii85 string.
2. Select 'Encode' to convert to Ascii85.
3. Select 'Decode' to convert back.
4. Copy the result.

## Example Input
```
Hello World
```

## Example Output
```
<~87cURD]i,"Ebo80~>
```

## Code Samples
### Python
```python
import base64
encoded = base64.a85encode(b'Hello World')
print(encoded)
```

## FAQ
### What are <~ and ~>?
These are the standard delimiters used by Adobe to mark the start and end of an Ascii85 string. I include them by default.

### What does 'z' mean?
If the data has four null bytes (00 00 00 00) in a row, Ascii85 compresses them to a single 'z' character to save space.

### Is it better than Base64?
It's more efficient (smaller output), but it uses characters like quote marks and backslashes that can be tricky in some systems. Base64 is safer; Ascii85 is smaller.

## Related Tools
- base64
- uuencoding

