NavVastram Inventory V43 – Mahajan Dashboard, Bill-wise Payments & Cheque Register

Backup V42 first. Extract ZIP and replace index.html, manifest.json, sw.js and README.txt in GitHub repository root. Refresh app. Do NOT clear browser site data/localStorage. Existing storage key remains navvastram_inventory_v2.

Changes:
1. Dealer tab is now presented as Mahajan Khata with four actions: Mahajan Ko Bhugtan, Udhar Kharid, Mahajan Khata, Naya Mahajan Jore. Existing dealer/supplier records are retained.
2. Mahajan payment shows oldest outstanding Purchase Register invoice. FIFO payment distributes across oldest unpaid invoices; Bill Wise Bhugtan allows partial payment against a selected invoice. Payment mode and remarks are saved.
3. Cheque issue register is integrated into Mahajan payment. It records amount, payee/party, due date, cheque number, bank and remarks. Pending cheque is highlighted in Mahajan payment and ledger. It does NOT reduce payable balance until clearance date is entered. Saving clearance date posts a CHEQUE payment on that date.
4. Udhar Kharid records payable in Mahajan ledger. For stock quantity/item purchase use Purchase Register; this direct entry is only for account adjustment.
5. Cheque records are included in local backup data.

Notes: Bill-wise outstanding is based on Purchase Register invoices. Older general payments without invoice links are applied FIFO for display. Opening balance is shown separately and any excess FIFO payment is recorded as unallocated/opening-balance payment.

Checks: JavaScript syntax and ZIP integrity. Actual mobile workflow testing remains to be done.
