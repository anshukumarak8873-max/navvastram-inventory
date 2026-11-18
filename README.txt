NavVastram Inventory V32 - Cash Realized Profit Update

Files: index.html, manifest.json, sw.js, README.txt

New accounting behavior:
- Inventory stock is reduced when a bill is completed, whether cash or credit.
- Cash/Nagad bills count the full bill total as received.
- Khata bills count only the amount actually received at billing time.
- Later customer payments are allocated to that customer's oldest outstanding bills first (FIFO).
- Each invoice's cash-basis result = amount collected against that invoice minus its recorded purchase cost.
- Amount collected below cost appears as unrecovered cost / negative cash-basis result; only receipts above cost become realized profit.
- The report shows total sales, total received, today's received amount, today's cash-basis profit/cost recovery, total outstanding, total cost, and estimated gross profit if all invoices are fully paid.
- Manual billing purchase cost rules are unchanged: Normal = MRP x 0.50 x 0.91; NET = MRP x 0.80. Barcode items use saved purchase price.

Important:
- Existing localStorage key remains navvastram_inventory_v2.
- Back up before replacing files. Do not clear browser site data.
- Customer payment allocation to bills uses oldest-first FIFO. Payments not matched to invoice balances remain as unapplied account balance.
- This is a cash-realization management view, not statutory accounting or tax advice.
