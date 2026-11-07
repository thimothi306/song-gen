# 🎶 Telugu Song Sheet Generator (A4 – Print Ready)

A clean and fast web tool to generate Telugu church song sheets for printing.
Add songs → reorder → auto-fit → print in perfect A4 layout.

🔗 Live Demo: https://livinghope-songsheetgen.netlify.app/

## Features

- Add songs with multiline lyrics
- Auto title from first lyric line
- Drag & drop reorder
- Edit & delete songs
- LocalStorage auto-save
- 1 or 2 column layout
- Adjustable font size & line height
- Auto-fit songs into selected number of pages
- A4 print-optimized (no margins / clean layout)

## Service list import (first stage)

Open [`service-import.html`](./service-import.html) to paste a service plan or upload an image. It can run Telugu/English OCR in the browser, then organizes the date, song entries, message, and offering into editable fields. Review the extraction and save the draft in your browser before proceeding. OCR needs an internet connection to load the library and language data.

This first stage does not fetch song lyrics or add songs to the print sheet yet. The next stage can build on the reviewed song list to provide lyric search suggestions and a confirmation flow.

## Project Structure

```
/
├── index.html          # Main application (UI + JS + CSS)
├── service-import.html # Service list import and OCR
└── sitemap.xml         # For SEO (Netlify)
```

## How to Run Locally

No server required. Open `index.html` for the song sheet generator or `service-import.html` for the importer.

## How It Works

- Songs in the generator are stored in localStorage
- HTML5 drag-and-drop is used for sorting
- Dynamic page generation is handled through JavaScript
- Auto-fit logic chooses font size based on song count and target pages
- Print view uses a hidden container and print CSS
