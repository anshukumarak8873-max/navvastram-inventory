NavVastram Inventory V21 – Manual Quick Entry

V21 changes requested for Manual Billing:
- Removed the Item Name / Design field completely.
- Selecting a clothing category image immediately opens the MRP, Quantity, Discount and Rate section.
- The selected category is used as the manual item name in the bill.
- Discount buttons and their two-column arrangement are unchanged from V20.

Existing V20 functionality and data storage are preserved, including barcode/manual shared cart, ledgers, profit calculations, NET rules and inventory behavior.

Profit rules:
- Normal Manual item purchase price = MRP × 0.50 × 0.91.
- NET Manual item purchase price = MRP × 0.80.
- Purchase price is based on MRP, not the selling rate.
- Manual items do not reduce inventory stock.
- NET items are exempt from bill-level discount allocation.

Files: index.html, manifest.json, sw.js, README.txt

Update safely:
1. Export a backup from the app first.
2. Extract this ZIP.
3. Replace all four files in the GitHub repository root.
4. Commit changes and reopen the website. Do not clear browser site data.
