🎶 Telugu Song Sheet Generator (A4 – Print Ready)

A clean and fast web tool to generate Telugu church song sheets for printing.
Add songs → reorder → auto-fit → print in perfect A4 layout.

🔗 Live Demo: https://livinghope-songsheetgen.netlify.app/

✨ Features

Add songs with multiline lyrics

Auto title from first lyric line

Drag & drop reorder

Edit & delete songs

LocalStorage auto-save

1 or 2 column layout

Adjustable font size & line height

Auto-fit songs into selected number of pages

A4 print-optimized (no margins / clean layout)

📂 Project Structure
/
├── index.html      # Main application (UI + JS + CSS)
└── sitemap.xml     # For SEO (Netlify)

▶️ How to Run Locally

No server required
Clone the repo:git clone https://github.com/thimothi306/song-sheet-generator.git
Open:
index.html


🧠 How It Works (Short Technical Details)

Songs stored in localStorage

HTML5 drag-and-drop for sorting

Dynamic page generation through JavaScript

Auto-fit logic chooses font size based on song count + target pages

Print view uses a hidden container + print CSS
