# Mime Extension Utils

A simple utility library to convert between file MIME types and their extensions, and vice-versa.

## Installation

To install the package, run the following command:

```bash
npm install mime-extension-utils

```

Usage

This package provides two main functions:

extension(mimeType: string): string | undefined: Returns the file extension for a given MIME type.

mineType(extension: string): string | undefined: Returns the MIME type for a given file extension.

Example

```typescript
import { getExtensionFromMime, getMimeTypeFromExtension } from "mime-extension-utils";

// Get file extension from MIME type
const extension = getExtensionFromMime("image/jpeg");
console.log(extension); // Output: ".jpeg"

// Get MIME type from file extension
const mimeType = getMimeTypeFromExtension(".jpeg");
console.log(mimeType); // Output: "image/jpeg"
```

API

1. getExtensionFromMime(mimeType: string): string | undefined
   Takes a MIME type as input and returns the corresponding file extension. If the MIME type is not found, it returns undefined.

Example:

```typescript
const ext = getExtensionFromMime("audio/mpeg");
console.log(ext); // Output: ".mp3"
```

2. getMimeTypeFromExtension(extension: string): string | undefined
   Takes a file extension as input and returns the corresponding MIME type. If the extension is not found, it returns undefined.

Example:

```typescript
const mime = getMimeTypeFromExtension(".mp4");
console.log(mime); // Output: "video/mp4"
```

Supported MIME Types and Extensions

The library supports a wide range of MIME types and file extensions, including but not limited to:

.aac - audio/aac
.abw - application/x-abiword
.apng - image/apng
.arc - application/x-freearc
.avif - image/avif
.avi - video/x-msvideo
.azw - application/vnd.amazon.ebook
.bin - application/octet-stream
.bmp - image/bmp
.bz - application/x-bzip
.bz2 - application/x-bzip2
.cda - application/x-cdf
.css - text/css
.csv - text/csv
.doc - application/msword
.docx - application/vnd.openxmlformats-officedocument.wordprocessingml.document
.eot - application/vnd.ms-fontobject
.epub - application/epub+zip
.gif - image/gif
.htm, .html - text/html
.ico - image/vnd.microsoft.icon
.ics - text/calendar
.jpeg, .jpg - image/jpeg
.js, .mjs - text/javascript
.json - application/json
.mp3 - audio/mpeg
.mp4 - video/mp4
.mpeg - video/mpeg
.pdf - application/pdf
.png - image/png
.svg - image/svg+xml
.tar - application/x-tar
.tif, .tiff - image/tiff
.txt - text/plain
.wav - audio/wav
.webm - video/webm
.zip - application/zip

And many more!

Contributing

Contributions are welcome! If you find a bug or want to request additional MIME types or extensions, feel free to open an issue or submit a pull request.

License

This project is licensed under the ISC License.
