NavVastram Inventory V20 – Exact Manual Billing Theme

V20 is based on the four-file V19 app package and reuses the user's earlier Thermal Bill Maker interface.

Manual System changes:
- Replaced the plain category dropdown with the same image-button category grid.
- Reused the original category names and embedded clothing images.
- Reused the original green/gold visual palette, image tile borders, selected tile treatment, and responsive grid.
- The selected category is shown clearly below the image buttons.
- Existing editable Rate, discount buttons, purchase-price rules, NET exemption, shared Barcode/Manual cart, ledgers, profit calculation and stock behavior remain intact.

Profit rules:
- Normal Manual item purchase price = MRP × 0.50 × 0.91.
- NET Manual item purchase price = MRP × 0.80.
- Purchase price is based on MRP, never on the entered selling rate.
- Manual items do not reduce inventory stock.
- NET items are exempt from bill-level discount allocation.

Files: index.html, manifest.json, sw.js, README.txt

Update:
1. Export a backup in the app first.
2. Extract this ZIP.
3. Upload and replace all four files in the GitHub repository root.
4. Commit changes and reopen the website. Do not clear browser site data.
