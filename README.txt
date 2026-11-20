NavVastram Inventory V34 - PIN Protected Customer / Dealer Delete

Files: index.html, manifest.json, sw.js, README.txt

V34 changes:
- Added a Delete option to each Customer record in Customer Ledger.
- Added a Delete option to each Dealer record in Dealer Ledger.
- Before either delete action, the app asks for the 6-digit PIN: 331223.
- Incorrect PIN or Cancel leaves the record unchanged.
- A second confirmation is shown before deletion.
- Deletion is a soft-delete/archive: the Customer or Dealer is removed from active lists and new billing/supplier selection, but existing bills, ledger entries, purchase history, and balances remain saved for historical records.
- Deleted records are retained in local backup data with a deletedAt marker.

Existing features preserved:
- localStorage key remains navvastram_inventory_v2.
- V33 invoice fixes remain: no dashed line between item rows, duplicate category names normalized on invoice, amounts displayed in whole rupees.
- Cash-realized profit logic and purchase register retained.

Update steps:
1. Download and extract this ZIP.
2. Back up your current four files and your app data before updating.
3. Replace index.html, manifest.json, sw.js, README.txt in the GitHub repository root.
4. Wait for GitHub Pages to publish, then reopen the app.

IMPORTANT:
- Do not clear browser Site Data / App Data; local inventory data is stored locally.
- PIN protection is an in-app safeguard, not strong security against someone who can inspect or modify the app source.
- Test with one sample customer/dealer first. Verify that old bills and ledger history remain visible.
