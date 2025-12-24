# Inventory Business Logic

## Inventory Accounting
Inventory is calculated using transaction-based accounting:

Current On-Hand = Starting Inventory + Σ(Transaction Quantities)

## Transaction Types
- RECEIVE: Positive quantity
- SALE: Negative quantity
- MOVE: Zero quantity
- ADJUST: Positive or negative
- CYCLE COUNT: Adjustment based on physical count

## Replenishment Logic
Reorder Point = (Average Daily Demand × Lead Time) + Safety Stock

Reorder alerts trigger when on-hand inventory falls below ROP.
