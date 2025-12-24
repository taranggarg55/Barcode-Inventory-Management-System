# Airtable Base Schema

## Tables

### Items (SKU Master)
- SKU (Primary)
- Product Name
- Category
- Barcode Value
- Unit Price
- Active

### Stores
- Store ID (Primary)
- Region

### Locations
- Location ID (Primary)
- Store (Linked)
- Zone
- Aisle
- Shelf
- Bin
- Location Barcode

### Transactions
- Transaction ID
- Timestamp
- Transaction Type
- Store
- Location
- SKU
- Quantity (signed)
- User
- Reason Code
- Notes

### Live Inventory
- Store
- SKU
- Starting Inventory
- Net Movement (Rollup)
- Current On Hand
- Snapshot Inventory
- Variance
- Reorder Point
- Reorder Alert
