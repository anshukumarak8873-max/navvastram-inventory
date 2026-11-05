NavVastram Inventory V22 – Thermal Bill Maker Manual Layout

Manual Billing layout updated to follow the original Thermal Bill Maker flow:
- Image category selection and selected-category strip.
- MRP and Quantity in one row.
- Original 3-column discount button layout: 30% OFF full-width, NET full-width, then remaining discount buttons in 3 columns.
- Pressing a discount button immediately adds the manual item to the bill, like the original Thermal Bill Maker.
- No separate Item Name input or visible Rate/Purchase Price form section.

Profit and purchase-cost rules from the V21 inventory system are retained:
- Normal manual item purchase cost = MRP × 50% × 91%.
- NET manual item purchase cost = MRP × 80%.
- Manual items do not reduce inventory stock.
- Barcode and manual items continue sharing the same bill cart.

Update safely:
1. Export/keep a backup of your current app data first.
2. Replace all four root files in your GitHub repository with these files.
3. Do not clear browser site data; existing local storage key navvastram_inventory_v2 is retained.
