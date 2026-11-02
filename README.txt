NAVVASTRAM INVENTORY - MOBILE TEST VERSION

Files:
- index.html: Inventory app
- manifest.json: Installable web-app settings
- sw.js: Basic offline cache

Features in this first test build:
1. Add item: name, purchase price, sale price, MRP, quantity, remarks.
2. Assign barcode by camera scan or manual entry.
3. Search inventory by name/barcode; scan barcode to search.
4. Edit item, delete item, adjust stock.
5. Test sale: scan/type barcode and reduce quantity.
6. Export/import JSON backup.

Important:
- This is a mobile-friendly PWA prototype, not a compiled Android APK.
- Camera access generally requires HTTPS or localhost and browser camera permission.
- Built-in BarcodeDetector support depends on the Android browser/device. If unavailable, manual barcode entry remains available.
- Data is currently stored in this browser on this device (localStorage). Do not clear browser data before exporting a backup.
- Google Drive sync, real billing integration, return workflow, and production-grade database migration are not included yet.
- To install as an app: host these files on an HTTPS site, open in Chrome, then use menu > Add to Home screen / Install app.
