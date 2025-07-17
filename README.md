# ISBN-13 QR Code Generator

A simple, fast web application for generating QR codes from 13-digit ISBN numbers with real-time validation.

## Features

- **Real-time ISBN-13 Validation**: Validates 13-digit ISBN numbers with proper check digit verification
- **978/979 Prefix Validation**: Ensures ISBNs start with valid prefixes
- **Instant QR Code Generation**: Creates scannable QR codes immediately upon entering a valid ISBN-13
- **Clean Interface**: Bootstrap-based responsive design optimized for quick data entry
- **Screen Scanning Optimized**: QR codes sized and styled for easy scanning directly from the screen
- **Input Validation**: Smart input filtering prevents invalid characters and provides visual feedback

## Usage

1. **Enter ISBN-13**: Click into the text field and enter any 13-digit ISBN number
   - Supports formats: `978-0-123456-78-9` or `9780123456789`
   - Must start with 978 or 979 prefix
   - Text auto-selects when clicking into the field for quick replacement

2. **Validation**: The system automatically validates your ISBN-13
   - ✅ Green checkmark for valid ISBN-13 numbers
   - ❌ Red X for invalid ISBN-13 numbers
   - Real-time feedback as you type

3. **Scan QR Code**: Once validated, scan the generated QR code directly from your screen
   - QR code contains the clean ISBN-13 number (digits only)
   - Compact 90px size optimized for mobile scanning

4. **Clear**: Use the "Clear" button to reset and enter a new ISBN-13

## Supported ISBN Format

### ISBN-13 (13 digits only)
- Standard format: `978-0-123456-78-9`
- Compact format: `9780123456789`
- Must start with 978 or 979 prefix
- Uses modulo 10 check digit algorithm

## Technical Details

- **Frontend**: HTML5, CSS3, Bootstrap 5.3.2, JavaScript
- **QR Generation**: QRious library v4.0.2
- **Validation**: Custom ISBN-13 check digit algorithm with 978/979 prefix validation
- **No Backend Required**: Runs entirely in the browser
- **No Data Storage**: All processing happens client-side

## File Structure

```
isbn13-qr-generator/
├── index.html          # Main application file
└── README.md          # This documentation
```

## Installation

1. Download the `index.html` file
2. Open in any modern web browser
3. No additional setup or dependencies required

## Browser Support

- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge
- Any modern browser with JavaScript enabled

## Features in Detail

### Input Validation
- Automatic character filtering (only allows digits, hyphens, and spaces)
- Real-time ISBN-13 format detection
- Mathematical check digit validation with 978/979 prefix requirement
- Visual feedback with icons

### QR Code Generation
- High-quality QR codes with error correction level M
- Black on white for maximum contrast
- Optimized size for screen scanning
- Instant generation upon validation

### User Experience
- Auto-focus on page load
- Text selection on field click
- Debounced input processing (200ms)
- Clear error messaging
- Responsive design for mobile and desktop

## Contributing

This is a standalone HTML application. To modify:

1. Edit the `index.html` file directly
2. Test in multiple browsers
3. Ensure ISBN validation accuracy

## License

Open source - feel free to use and modify as needed.

## Support

For issues or questions:
- Check that your ISBN-13 is correctly formatted and starts with 978 or 979
- Ensure JavaScript is enabled in your browser
- Try clearing the cache and reloading the page