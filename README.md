# Barcode-Based Inventory Management System

## Overview
This project implements a barcode-driven inventory management system that tracks SKU-level inventory movements across stores and locations. The system uses transaction-based inventory accounting, automated reconciliation, and demand-driven replenishment logic to mirror real-world WMS/ERP inventory control.

## Key Features
- Barcode-style transaction ledger (RECEIVE, SALE, MOVE, ADJUST, CYCLE COUNT)
- Automated inventory roll-up using signed quantities
- Real-time on-hand inventory calculation
- Reconciliation against inventory snapshots
- Reorder point, safety stock, and days-of-supply logic
- Airtable automations to eliminate manual linking errors

## System Architecture
Inventory is never manually updated. All stock levels are derived from transaction history:

Starting Inventory  
+ Receipts  
− Sales  
± Adjustments  
= Current On-Hand

## Tools Used
- Airtable (Inventory system, automations, dashboards)
- Spreadsheet-based sample data (for demonstration)
- Inventory planning logic (ROP, safety stock)

## Business Logic
- Positive quantities increase inventory
- Negative quantities decrease inventory
- Composite Store–SKU keys ensure correct record matching
- Reorder alerts are triggered based on demand and lead time

## Outputs & Planning Views

### Inventory Transactions (Barcode Scans)
![Transactions](Screenshots/transactions_table/transactions_table1.png)

### Live Inventory Calculation
![Live Inventory](Screenshots/live_inventory/live_inventory2.png)
![Live Inventory](Screenshots/live_inventory/live_inventory1.png)

### Reorder Decisions
![Reorder](Screenshots/reorder_alert/reorder_alert.png)

### Automation
![Automation](Screenshots/automation_logic/automation_logic1.png)
![Automation](Screenshots/automation_logic/automation_logic2.png)


### Auto Linked Transactions
![Auto Linked Transactions](Screenshots/auto_linked_transaction/auto_linked_transaction1.png)
![Auto Linked Transactions](Screenshots/auto_linked_transaction/auto_linked_transaction2.png)


## Use Case
Designed for retail stores, warehouses, or shared inventory environments requiring traceability, auditability, and demand-driven replenishment decisions.

## Author
Tarang Garg
