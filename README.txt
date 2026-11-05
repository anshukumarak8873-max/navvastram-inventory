NavVastram Inventory V24 - Voice Similar-Name Matching

Changes:
- Voice search for village names now ranks similar saved village names and displays selectable suggestions.
- Voice search for customer names ranks similar saved customer names and displays selectable suggestions.
- Added to both Customer Ledger search and Billing (Khata) village/customer selection.
- Uses up to 5 speech-recognition alternatives where supported; user confirms the correct saved name by tapping it. No uncertain automatic selection.
- Existing inventory, billing, profit, discount, barcode, and manual billing logic is retained.

Update steps:
1. Export/backup your current app data first.
2. Extract this ZIP.
3. Replace all four files in the GitHub repository root: index.html, manifest.json, sw.js, README.txt.
4. Commit changes and reopen the app.

Important: Do not clear browser site data. Existing localStorage key navvastram_inventory_v2 is preserved.
Voice recognition availability depends on browser/device support and microphone permission.


V25 update:
- Removed the Gross Profit row from the customer-facing printed PNG invoice.
- Estimated per-item and bill profit remain visible inside the billing screen for the shop owner.
- Profit reporting and saved bill profit records are retained.
- Existing localStorage data key and all other app data are preserved.

Update safely:
1. Export a backup from the app before replacing files.
2. Replace all four files in the GitHub repository root.
3. Do not clear browser site data.


Version 26 - Purchase Register
- One supplier invoice can include multiple existing inventory items.
- Saving a purchase increases each selected item stock and updates its purchase rate.
- Purchase Invoice total and paid amount are posted to the selected wholesaler ledger; remaining balance stays payable.
- Purchase history is stored in the existing localStorage key navvastram_inventory_v2 and included in backup/restore.
