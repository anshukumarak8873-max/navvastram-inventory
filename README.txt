NavVastram Inventory V27 — Purchase Register Visibility + Gross Purchase Cost Report Fix

Files: index.html, manifest.json, sw.js, README.txt

Changes:
1. Purchase Register is now available from a prominent button above the tabs and remains in the tab list. Opening it refreshes supplier choices, item rows, and purchase history.
2. Report purchase cost uses each saved bill-line cost snapshot. For older bills missing costAmount, it falls back to purchaseCostPerUnit; manual lines use the established normal (MRP × 0.455) or NET (MRP × 0.80) formula; barcode lines fall back to current product purchase price only when no historical cost snapshot exists.
3. Service worker now calls skipWaiting() so a new GitHub Pages version can activate without waiting for all old tabs to close.
4. Existing localStorage key remains navvastram_inventory_v2.

Important: Make a backup before replacing files. Do not clear browser site data. Supplier must first exist in Dealer account; purchase invoice supports multiple existing inventory items.
