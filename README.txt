NavVastram Inventory V35 - Cash Basis Daily Report

Update from V34. Includes the V34 PIN-protected Customer/Dealer delete and all existing app modules.

Daily report rules requested by shop owner:
1. Today's Total Sales = today's new bill totals + collections received today against older bills (old dues). Initial payments on today's bills are not counted twice.
2. Today's Profit/Loss = all actual payments received today (including old dues) minus the purchase cost of all items sold on today's bills.
3. Example: ₹10,000 bill, cost ₹8,000, received ₹5,000 today => today's result -₹3,000. A later ₹2,000 old-dues collection on another day => that later day's result +₹2,000 if no new stock cost was sold that day.
4. Example: same day ₹5,000 fully paid sale with ₹4,000 cost gives +₹1,000; ₹4,000 sale with ₹3,200 cost and ₹2,000 received gives -₹1,200; daily net = -₹200.
5. Example: ₹14,000 today's new bills + ₹4,000 received against older bills = ₹18,000 today's Total Sales. The old payment is included in today's receipts/profit, and not counted as a new bill.

Customer payments continue to be allocated to oldest outstanding bills (FIFO). Lifetime cash-basis net profit remains total collections applied to bills minus total cost of goods sold.

IMPORTANT: localStorage key remains navvastram_inventory_v2. Back up the app data and all four files before replacing. Do not clear browser site data.
Files: index.html, manifest.json, sw.js, README.txt


V36 Sales Dashboard & Date Range Reports
- Daily Sales and Monthly Sales count only actual payments received (Cash/UPI/Bank), including customer khata payments and old outstanding collections. Credit-only bill value is not counted as Sales until payment is received.
- Daily/period Profit-Loss = payments received during the selected period minus full purchase cost of goods sold during that period. Old dues received later do not deduct old purchase cost again.
- Reports include Daily, Month-to-date, and a custom inclusive From/To date range with a daily breakdown.
- Existing localStorage key is preserved: navvastram_inventory_v2. Back up data before replacing files.
