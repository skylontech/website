# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static single-page application (SPA) website for SkylonTech Inc., showcasing their AI products and services. The site is built with vanilla HTML, JavaScript, and TailwindCSS (loaded via CDN).

## Architecture

- **Single HTML file**: `index.html` contains all content and functionality
- **Client-side routing**: JavaScript-based page switching without server requests
- **Styling**: TailwindCSS via CDN with custom brand colors
- **Assets**: Logo (`SkylonLogo.png`) and app screenshot (`Screenshot_Whimsical_Weather.jpg`)

## Brand Colors

- Dark Blue: `#1a3b4a`
- Orange: `#ff7a47`
- Teal: `#16888d`
- Base Background: `#e2f2f5`

## Development Commands

Since this is a static website with no build process:

```bash
# Serve locally with Python
python3 -m http.server 8000

# Or with Node.js http-server (if installed)
npx http-server

# Or open directly in browser
open index.html  # macOS
xdg-open index.html  # Linux
```

## Key Features

1. **Multi-page SPA structure**: Home, Portfolio, Privacy Policy & Terms, Contact
2. **Responsive design**: Mobile menu with hamburger navigation
3. **Page state management**: JavaScript-based routing using CSS classes
4. **Privacy Policy and Terms**: Comprehensive legal pages for the Whimsical Weather app

## Important Notes

- The Google Play Store link in the Portfolio section is currently a placeholder (`href="#"`)
- All content is contained within `index.html` - no external JavaScript or CSS files
- Navigation is handled via `showPage()` function that toggles visibility of sections
- Mobile menu automatically closes after navigation