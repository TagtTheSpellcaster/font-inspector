![Version](https://img.shields.io/badge/version-1.4.1-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-browser%20%7C%20PWA-lightgrey)
![Built with HTML](https://img.shields.io/badge/built%20with-HTML-orange)
![Status](https://img.shields.io/badge/status-stable-brightgreen)

# Font Inspector & Glyph Analyzer

A single-page, browser-based web application for inspecting, analyzing, and testing OpenType fonts (`.ttf`, `.otf`, `.woff`, `.woff2`). Built using **OpenType.js** and **Tailwind CSS**, it allows font designers, developers, and typographers to deeply inspect glyphs, Unicode ranges, OpenType GSUB features, and alternates in real-time.

## Key Features

* **Client-Side Font Parsing**: Drag-and-drop or upload custom font files (`.ttf`, `.otf`, `.woff`, `.woff2`). Everything is processed locally in your browser—no backend or data transmission.

* **Full Character Map & Glyph Inspector**: Browse every character mapped in the font's Unicode table (`CMAP`), displaying Hex (`U+XXXX`) and Decimal codes side-by-side.

* **Side-by-Side Standard Comparison**: Compare font glyphs directly against a standard fallback font (`Arial / sans-serif`) to detect missing glyphs or visual deviations.

* **OpenType GSUB Feature Analysis**:

  * Automatically detects substitution tables (`GSUB`) including **Ligatures** (`liga`, `clig`, `dlig`, `hlig`), **Contextual Alternates** (`calt`), **Swashes** (`swsh`), **Fractions** (`frac`), and **Stylistic Sets** (`ss01` - `ss20`).

  * Interactive feature toggles that dynamically control rendering using CSS `font-feature-settings`.

* **Alternate Glyphs & Variants Detection**: Programmatically inspects OpenType Type 1 (Single) and Type 3 (Alternate) substitutions, displaying glyph alternates directly inside the character map table.

* **Interactive Live Text Preview**:

  * Test custom input phrases with full font-feature support.

  * Quick-preset buttons for testing pangrams, complex ligatures (`fi`, `fl`, `ffi`, `ffl`, `st`), and numeric fractions.

  * Font sizing controls.

* **Instant Search & Pagination**: Search by Unicode hex code, character, decimal value, glyph name, or OpenType variant name with fast pagination for smooth performance on large fonts.

## Live Demo

You can host this project directly on **GitHub Pages**.

1. Fork or clone this repository.

2. Enable GitHub Pages under **Settings > Pages** and select the `main` branch.

3. Open your custom `.github.io` URL.

## Technology Stack

* **HTML5 & Vanilla JavaScript (ES6+)**

* [**Tailwind CSS**](https://tailwindcss.com/) (via CDN) – UI styling

* [**OpenType.js**](https://opentype.js.org/) – In-browser font parsing & GSUB table inspection

* [**Lucide Icons**](https://lucide.dev/) – Minimalist UI iconography

* **CSS `font-feature-settings` & `FontFace` Web API** – Dynamic font loading and real-time feature application

## Local Quickstart

Since this is a client-side single-file application (`index.html`), no node packages or build steps are required.

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/font-inspector.git
   ```

2. Open `index.html` directly in any modern web browser.

## License

This project is licensed under the **MIT License**.
