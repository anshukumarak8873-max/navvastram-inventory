NavVastram Inventory V38 - Professional Buttons & Customer Ledger UI

Update from V37. Existing data storage key is preserved:
navvastram_inventory_v2

Customer Khata screen redesign:
- Main customer screen now opens with two primary actions: Bhugtan Prapti and Khata Dekhen.
- Separate lower actions: Naya Grahak Jode and Grahak ka Vivran Badlein.
- Bhugtan Prapti lets the user choose a customer, enter amount/date/payment mode/remark, and save the receipt.
- A separate Payment Receipt List is available from the payment screen, with date-range and customer-name filters.
- Khata Dekhen shows customer search/list and the selected customer's ledger.
- Customer details edit form supports Name, Village/Address, Khata Page and Mobile Number updates.
- Existing customer ledger entries, bill records and customer IDs are preserved when basic details are edited.
- Existing voice search, manual credit entry, customer delete PIN, bill delete, sales reports and inventory modules remain included.

UI:
- Buttons have a cleaner, consistent professional website-style treatment with improved spacing, focus states and active feedback.
- Customer ledger main actions are arranged for mobile screens.

Important:
1. Export a data backup before replacing files.
2. Replace all four root files: index.html, manifest.json, sw.js, README.txt.
3. Do not clear browser site data or localStorage; that may erase inventory and customer records.
4. This is a local/offline-first app; payment list shows entries recorded in this app's customer ledger.
5. Verify the new interface on the actual phone after deployment. Browser syntax and archive integrity checks do not equal full device testing.


V39 Modification:
- Payment Receipt screen now has voice search for Village and Customer Name, matching the Khata Dekhen voice matching workflow.
- Voice village recognition ranks similar village names; choosing one filters the customer list.
- Voice customer recognition ranks similar customer names within the selected village and shows village/balance details.
- Clicking “भुगतान दर्ज करें” now asks for confirmation with customer, village, amount, date and payment mode. The ledger entry is saved only after OK. Cancel leaves data unchanged.
- Existing localStorage key navvastram_inventory_v2 is preserved.
