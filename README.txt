NavVastram Inventory V46 — Flexible Savings / Deposit Entries

Replace the four repository-root files: index.html, manifest.json, sw.js, README.txt.

Changes:
- Post Office deposits can be entered multiple times during a month, using the actual amount each time (e.g. ₹100, ₹500, etc.).
- SIP can be entered on any actual transaction date; no fixed date is imposed.
- Every deposit is saved as a separate dated transaction.
- Monthly dashboard totals all Post Office and SIP transactions and shows remaining monthly target (Post Office ₹9,000; SIP ₹5,000).
- Existing navvastram_inventory_v2 localStorage key and previous records are preserved.

Before updating, export an in-app backup. Do not clear browser Site Data. Source syntax and ZIP integrity checked; mobile workflow not tested on a physical device.


V55 Dashboard Update:
- Professional dashboard layout.
- Total summary details are hidden until the user opens 'Kul Jankari Dekhen'.
- Large Expense and Savings actions are placed at the top.
- Expense details are hidden until 'Kharch Vivaran Dekhen' is opened.
- Existing localStorage data key is preserved; take a backup before updating and do not clear browser site data.
