# QR Maker

![Version: 1.3.0](https://img.shields.io/badge/version-1.3.0-557BD9?style=plastic&labelColor=555) ![HTML5: single-file](https://img.shields.io/badge/HTML5-single--file-E86C19?style=plastic&labelColor=555) ![Offline: ready](https://img.shields.io/badge/offline-ready-238636?style=plastic&labelColor=555) ![Portable: yes](https://img.shields.io/badge/portable-yes-238636?style=plastic&labelColor=555) ![Languages: 4](https://img.shields.io/badge/languages-4-557BD9?style=plastic&labelColor=555) ![Export formats: 18](https://img.shields.io/badge/export%20formats-18-557BD9?style=plastic&labelColor=555)

QR Maker creates customizable, static Quick Response (QR) codes. It runs from one HTML5 file, without installation or Internet access.

## Live application:

[https://firerayo.github.io/QR-Maker/](https://firerayo.github.io/QR-Maker/)

## Features

| Feature | Description |
| --- | --- |
| 60 content types | URLs, text, calls, SMS, email, Wi-Fi (including enterprise networks), vCard, MeCard, vCard Plus, coordinates, directions, and calendar events. |
| Social links | WhatsApp, Telegram, Signal, Facebook, X, Instagram, TikTok, LinkedIn, Spotify, Tripadvisor, YouTube, Messenger, profiles, and link pages. |
| Media and files | Meeting links, app stores, PDFs, downloads, videos, MP3 audio, galleries, ebooks, and restaurant menus. |
| Business and payments | Forms, Google Forms, feedback, ratings, Google Reviews, Yelp, business pages, registration, queues, payment links, cryptocurrency, PIX, SEPA, coupons, tickets, and existing redirect URLs. |
| Structured data | Time-based one-time password (TOTP) setup, JSON, XML, CSV, product/equipment IDs, 2D product links, deep links, and custom content. |
| Appearance | Six module shapes, three corner styles, separate colors, linear/radial gradients, transparency, eight presets, and randomized styling. Save and reload a custom style. |
| Logos and frames | Add a logo with adjustable size and padding. Select frames and captions. Logo protection forces error correction H and may shrink the logo. |
| QR settings | Error correction L/M/Q/H; automatic or manual versions 1–40; automatic or manual masks 0–7; numeric, alphanumeric, or UTF-8 byte encoding; quiet-zone width. |
| Preview and checks | Live preview, encoded text, matrix/byte details, contrast warnings, and supported-browser readability checks. |
| Export | PNG, SVG, JPG, JPEG, WebP, BMP, GIF, TIF, TIFF, PPM, PGM, PBM, TGA, QOI, ICO, AVIF, PDF, and EPS. Select a file name and image resolution; copy a PNG or SVG text, or print. |
| Projects and tools | Import/export project JSON, reset projects, enable local history, and scan QR images on supported browsers. |
| Local project library | Save, search, open, and delete projects with labels, folders, media, dates, and planned print quantities. |
| Landing pages | Export a standalone HTML page with a title, description, and up to 20 HTTPS links. Publish it separately. |
| Interface | Light/Dark Neomorphism; English, Spanish, Italian, Brazilian Portuguese; About dialog. |

## Quick start

1. Download [`index.html`](index.html) from this repository.
2. Open the file in a modern browser.
3. Select a **Content type** and enter its details.
4. Adjust **Appearance** and **Advanced settings** as needed.
5. Check **Live preview** and select an **Image format**.
6. Select **Download QR image**.

**Example:** Select **Website / URL**, enter `https://github.com/FireRayo/`, and export a PNG.

## Limitations and compatibility

- QR codes are **static**. Destination editing, scan analytics, redirects, and hosted files require external services.
- Linked files and pages must already be hosted elsewhere.
- Scanning and visual checks require the browser’s `BarcodeDetector` API.
- AVIF encoding and large exports depend on browser support and memory.
- Resolution can reach **8192 px** for supported exports. BMP, GIF, TIFF/TIF, PPM/PGM/PBM, TGA, and QOI are limited to **4096 px**; EPS to **1024 px**; ICO to **256 px**.
- Contrast, styles, and logos affect scanning. Test exported QR codes before printing.

## Data and privacy

Generation and export run locally. No network calls, remote scripts, or analytics endpoints appear in the reviewed source.

Language, theme, saved styles, optional history, and saved library projects use browser `localStorage`. Exported images, JSON, and HTML remain on your device. Clear saved entries in the app or browser. TOTP secrets are excluded from history and library saves. Exported TOTP project JSON may contain its secret.

## Development and tests

Edit [`index.html`](index.html) directly. The repository has no build scripts, test suite, or continuous integration workflow. Test generated codes with an independent reader.

## Contributing and support

Report bugs or request changes through [GitHub Issues](https://github.com/FireRayo/QR-Maker/issues).

## License and credits

**Project license:** No repository-level `LICENSE` file was found. The complete application has no verified open-source license.

**Author:** Raymundo Ortiz ([FireRayo](https://github.com/FireRayo/)). The embedded engine credits [Kazuhiko Arase’s `qrcode-generator`](https://github.com/kazuhikoarase/qrcode-generator) under MIT. This does not license the complete application.
