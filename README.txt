NavVastram Inventory V19 – Manual Billing + Profit Calculation

Included files (upload all four to the GitHub repository root):
- index.html
- manifest.json
- sw.js
- README.txt

V19 changes:
1. Billing now has Barcode System and Manual System. Both add items to the same cart; switching systems does not clear the cart.
2. Manual item entry includes clothing categories, item/design name, MRP, quantity, discount buttons and editable selling rate.
3. Discount buttons are arranged as requested: 30%, 0% NET directly below, then 10%, 15%, 20%, 25%, 35%; separate side group: 40%, 45%, 50%.
4. The discount percentage below MRP updates from the actual editable selling rate.
5. Normal manual item purchase price = MRP × 0.50 × 0.91. Example: MRP ₹1,000 -> Purchase Price ₹455, even if the selling rate is ₹400.
6. NET manual item purchase price = MRP × 0.80. NET items are exempt from both item/bill-level discount allocation.
7. Entering a customer final amount automatically calculates the grand-total discount. The discount is allocated proportionally only to eligible non-NET items. If the requested final amount would reduce the NET items, the app warns and does not save the bill.
8. Manual items do not reduce inventory stock. Barcode-linked items continue to reduce stock as before.
9. Each bill stores purchase cost, final item amount and profit. The Reports page shows billing revenue, purchase cost and gross profit.
10. Existing localStorage key `navvastram_inventory_v2` is unchanged; customer/dealer ledgers and existing inventory data are retained.

Update:
1. Export a backup from the app before updating.
2. Extract this ZIP.
3. Upload and replace the four files in the GitHub repository root.
4. Commit changes and reopen the site. Do not clear browser site data.

Suggested tests:
- Normal manual item: MRP ₹1,000, choose 30%, then change Rate to ₹400. Purchase Price should remain ₹455 and base discount should show 60%.
- NET item: MRP ₹1,000, NET button. Purchase Price should be ₹800; grand-total discount must not reduce this line.
- Five eligible items at ₹100 each: enter Final Amount ₹450. BILL TOTAL should be ₹450 and ₹50 discount should be allocated across eligible items.
- Mix Barcode and Manual items in one cart. Manual item should not reduce inventory; Barcode item should continue to reduce inventory.
