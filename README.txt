NAVVASTRAM INVENTORY - V31 HYBRID BILL SCANNER (IMAGE + PDF)

New in V31:
1. Purchase Register bill scanner accepts JPG, PNG, and PDF files.
2. Multi-page PDF is supported: each page is rendered in the browser and OCR-processed sequentially (maximum 30 pages per PDF).
3. Browser OCR uses Tesseract.js with English + Hindi recognition.
4. PDF rendering uses PDF.js. First use requires internet to load PDF.js, its worker, Tesseract.js, and OCR language data.
5. OCR text remains editable. Existing invoice number/date and possible item-line extraction workflow is retained.
6. OCR is only a draft aid. User must review and correct supplier, invoice, item, quantity, rate, and payment before saving.
7. OCR does not automatically update stock or supplier ledger. Only the existing Purchase Save action does that.
8. JPG/PNG and Manual Purchase Entry remain supported if PDF/OCR fails.
9. Existing localStorage key is preserved: navvastram_inventory_v2.

LIMITATIONS:
- This is browser-side OCR, not a paid generative-AI API. No guaranteed extraction of complex tables, handwriting, blurry scans, or unusual invoice layouts.
- Scanned PDFs are processed page by page; large PDFs may take several minutes and use phone memory. Limit: 30 pages per PDF.
- First use and language-data download require internet. Manual Entry remains available offline.
- Item-line matching is best-effort. New articles should be created in Inventory first, then selected in Purchase Register.

INSTALL:
1. Take an in-app Backup first.
2. Extract this ZIP and upload/replace all four files in the GitHub repository ROOT: index.html, manifest.json, sw.js, README.txt.
3. Wait for GitHub Pages deployment, then close and reopen the site.
4. Do NOT clear browser site data. The existing inventory data key is unchanged.
