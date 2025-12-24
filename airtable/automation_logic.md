# Inventory Automation Logic

## Objective
Automatically link transactions to the correct inventory record and update on-hand inventory in real time.

## Method
- Create a composite Store–SKU key in Transactions and Live Inventory
- Trigger automation when Live Inventory Link is empty
- Find matching Live Inventory record using Store–SKU key
- Update Transaction with correct inventory link

## Result
- Zero manual linking
- No cross-store or cross-SKU contamination
- Real-time inventory accuracy
