NavVastram Inventory V16 – Item Discount & Bill Discount Allocation

Files: index.html, manifest.json, sw.js, README.txt

V16 changes:
- Invoice summary label changed from CURRENT BILL to BILL TOTAL.
- Every invoice item shows its MRP discount percentage directly below MRP.
- Customer Discount percentage is shown in brackets beside the discount amount.
- Bill-level Customer Discount is allocated proportionally across only those items whose MRP is higher than their original selling rate.
- Items whose MRP equals their selling rate are excluded from bill-level discount and their rates remain unchanged.
- Adjusted item rates and amounts are saved in the invoice, so the sum of item amounts equals the final BILL TOTAL (subject to currency rounding).
- Discount cannot exceed the combined selling value of eligible discounted items.
- Existing inventory, customer ledger, dealer ledger, billing, PNG share, PDF share, and stored data key are retained.

Update instructions:
1. Export a backup from the app first.
2. Extract this ZIP.
3. Upload and replace all four files directly in the GitHub repository root.
4. Commit changes, then reopen the website. Do not clear browser site data.
5. Test with (a) one item where MRP > selling rate and (b) one item where MRP = selling rate. Apply a customer discount and verify only the first item's rate reduces.

V16: Fixed effective item discount percentage, proportional paise-level bill discount allocation, final discount amount/percentage display, and MRP column spacing.
