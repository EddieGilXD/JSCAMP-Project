# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

Repository overview
- This repository is a minimal static site. It contains a single HTML entry point at index.html and no package manager or build/test/lint tooling.

Commands
- Preview in default browser (Windows PowerShell):
  - Open index.html with the system default browser
    
    Invoke-Item .\index.html

- Serve locally with a lightweight HTTP server (choose one):
  - Using Python (if installed)
    
    python -m http.server 5500
    
    Then open http://localhost:5500 in your browser.
  - Using Node.js (if installed)
    
    npx serve . -l 5500
    
    or
    
    npx http-server -p 5500

- Build/lint/test
  - No build, lint, or test commands are configured in this repository.

High-level architecture
- Single-page static site: index.html defines the document shell with Spanish metadata (lang="es") and the page title "DevJobs". There are no linked JavaScript or CSS assets and no application framework present.
