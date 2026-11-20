NavVastram Inventory V44 — Money Manager

Files: index.html, manifest.json, sw.js, README.txt
Update: replace the four files in the GitHub repository root.

New features:
- Separate Home and Shop cash expenses.
- Home and Shop clothing expenses by barcode or manual entry.
- Barcode clothing uses inventory purchase price and reduces stock; manual clothing entry uses the manually entered purchase price and does not change inventory.
- Staff salary ledger: add salary due, record multiple cash payments, and record clothing as salary payment at purchase price. Barcode clothing reduces stock.
- Fixed expenses: monthly EMI default ₹24,157 (suggested date 5th), manually entered CC account interest, bank charges and other fixed expenses.
- Savings/deposits tracked separately: Post Office target ₹9,000/month and SIP target ₹5,000/month.
- Month summary and date-filtered history.
- Existing data key navvastram_inventory_v2 is preserved; new records are included in backup/restore.
- Global navigation: opening any tab or money sub-screen automatically scrolls it into view.

Important:
1. Download and keep a backup from the app before replacing files.
2. Replace index.html, manifest.json, sw.js and README.txt in repository root.
3. Do not clear browser Site Data or app storage.
4. Data remains on this device/browser unless you manually export and store a backup.
5. This build has source/syntax checks only; test the flows with small sample entries first.
