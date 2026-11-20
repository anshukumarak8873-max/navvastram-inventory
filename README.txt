NavVastram Inventory V41 – Actual Profit, Payment Discount & Bill-wise Payments

Update: Backup V40 first. Replace index.html, manifest.json, sw.js and README.txt in the GitHub repository root. Refresh the app. Do NOT clear site data/localStorage. Data key remains navvastram_inventory_v2.

Accounting rules:
1. Bill Wise Profit/Loss = final bill amount minus full purchase cost of all goods in that bill.
2. Actual Profit for a bill = actual cash/UPI/bank amount received against that bill minus its full purchase cost. Discount/write-off is not cash and does not count as Sales.
3. General customer payment applies cash to oldest outstanding bills first (FIFO), then discount/write-off applies to remaining oldest dues.
4. Bill Wise Payment lets the operator select one unpaid bill and enter partial/complete cash received and a separate discount against that bill.
5. Payment/discount are separately recorded in customer ledger; only PAYMENT is included in Sales collections.
6. Discount reduces customer/bill outstanding but is excluded from Sales and cash receipts.

Testing note: JavaScript syntax check and ZIP integrity check performed. Browser/device end-to-end workflow and real thermal printer testing remain outstanding.
