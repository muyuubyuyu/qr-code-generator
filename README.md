# QR Code Generator (Online)

A small, clean single-file HTML tool to generate print-ready QR codes directly in the browser – perfect for price tags, product links, posters, and in-store use.

## Live Demo
You can use the QR Code Generator directly in your browser:

https://muyuubyuyu.github.io/qr-code-generator/


## Features
- **Generate QR codes from any URL**
- **Adjustable error correction level** (L / M / Q / H)  
  - Default: **H** (recommended for print & real-world use)
- **Adjustable margin (Quiet Zone)**  
  - Default: **0** (no white border)
- **Adjustable size (px)**  
  - Default: **512 px** (recommended 512–1024 px for price tags)
- **Automatically uses the smallest fitting QR version**  
  - No fixed version → adapts to URL length automatically
- **Live preview** inside the interface
- **PNG download** with smart filename  
  - Filename is auto-generated from the URL slug + `_qr.png`
- **Clear button** directly under the URL field  
  - Clears the input, resets preview, and focuses the URL field again

## Tech
- **Single file**: pure HTML, CSS, and JavaScript  
- QR generation powered by the well-known **qrcode** JS library (via CDN)

## How to Use
1. Clone the repository or download the file  
2. Open `index.html` in your browser (double-click)  
3. Paste a URL  
4. Click **Generate**  
5. Download the QR code as PNG

## Why These Defaults?
- **Error Correction H** provides the highest robustness (important for printed codes, scratches, folds, dirt).
- **margin = 0** is useful when placing the QR code inside custom layouts or price tag designs.
- **Automatic version selection** ensures long URLs always work without data overflow.

## Files
- `index.html` – the complete application

## CDN Note
The QR library is loaded via CDN:
- `https://cdn.jsdelivr.net/npm/qrcode/build/qrcode.min.js`

## License
Do whatever you want with it.
