# SCL Agency Name Scraper

A browser-based tool that automatically retrieves and extracts agency names from the UK REDCap SCL Agency Survey form and allows export in multiple formats.

The application uses a lightweight serverless proxy to fetch the survey HTML directly, eliminating the need for manual page-source copying.

## Usage

1. Go to  
   **https://pgspears.github.io/AgencyExtractor**

2. The application automatically loads the survey HTML via a secure proxy.

3. Agency names are extracted immediately and displayed under **Extracted Agencies**.

4. Use the export buttons to download the agency list in your preferred format.

No manual interaction with the REDCap survey page is required.

## Optional: View Source HTML

An optional toggle allows you to view the raw HTML returned by the proxy for transparency or debugging purposes. This is read-only and not required for normal use.

## Export Formats

- CSV  
- Excel (XLSX)  
- JSON  
- Text (TXT)  
- PDF  

## Settings

- Remove parenthetical text (enabled by default)  
- Show unique agencies only  
- Sort alphabetically  
- Include timestamp in exports  

## How It Works (Brief)

- A Cloudflare Worker fetches the REDCap survey HTML server-side.
- The browser app retrieves that HTML without CORS restrictions.
- Agency names are parsed directly from the returned document.
- No authentication, cookies, or simulated user interaction is required.

## Requirements

- Modern web browser (Chrome, Firefox, Edge, Safari)
- Internet connection (for CDN libraries: SheetJS, jsPDF, Google Fonts)

---

© 2025 Accelerate Solutions, LLC  

*Created with Claude Opus 4.5*
