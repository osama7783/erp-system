# MIKATAKNO ERP/WMS System

A full-stack ERP/WMS operational management system designed to support real business workflows for sales, purchasing, inventory, warehouse operations, fulfillment, barcode tracking, and internal company processes.

This repository represents a public/demo version of a larger ERP/WMS platform developed to organize business operations between administrators, employees, customers, suppliers, warehouses, and operational teams.

---

## Project Overview

MIKATAKNO ERP/WMS is built to manage the daily workflow of a trading, warehouse, and operational business environment.

The system focuses on connecting core business processes such as:

- Sales orders
- Purchase orders
- Inventory and stock tracking
- Warehouse operations
- Packing and fulfillment
- Pallets and container loading
- Barcode and QR traceability
- Excel import/export workflows
- Role-based access control
- Internal operational reporting

The main goal of the system is to reduce scattered manual work and provide a structured workflow for managing business operations from order creation to inventory tracking and fulfillment.

---

## Key Features

### Sales Management
- Sales order creation and management
- Customer-based sales workflows
- Sales order tracking
- Order status and operational follow-up
- Contextual Excel export for sales data

### Purchasing Management
- Purchase order creation and supplier tracking
- Supplier-based purchase workflows
- Purchase order lifecycle management
- Support for manual and file-based purchasing data

### Inventory & Warehouse Management
- Multi-warehouse inventory structure
- Stock balances and inventory movement tracking
- Warehouse/location-based stock visibility
- Inventory intake workflow concept for opening stock, manual intake, and factory-related stock entry
- Audit-friendly stock movement history

### Fulfillment & Packing Operations
- Packing plan workflow
- Pallet builder and pallet item allocation
- Support for single-SKU and mixed-SKU pallet concepts
- Container load management
- Packing list generation from real operational allocation records

### Barcode & Traceability
- Internal barcode/QR-based entity tracking
- Barcode support for products, orders, pallets, containers, and warehouse operations
- Scan/trace workflow concept for opening related operational records
- Barcode payloads based on internal identifiers instead of sensitive business data

### Import & Export
- Excel import/export workflows
- Operational data processing
- Export support for sales, purchases, inventory, packing lists, pallet contents, and container-related data
- Structured file-processing approach for business records

### User Roles & Permissions
- Role-based access control
- Admin, employee, warehouse, sales, purchasing, and auditor-style access patterns
- Permission-aware UI and backend protection
- Safe separation between read-only and operational actions

---

## Tech Stack

### Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS
- Responsive dashboard and operational UI
- Role-aware interface components

### Backend
- NestJS
- REST APIs
- Modular backend architecture
- Business workflow services
- Role-based access control
- Audit-safe operational logic

### Database
- PostgreSQL
- Prisma ORM
- Database migrations
- Relational data modeling for ERP/WMS workflows
- Inventory balances, movements, orders, pallets, containers, and operational records

### Processing & Automation
- Python
- FastAPI
- Excel import/export processing
- Operational file handling
- Data transformation workflows

### Infrastructure
- Docker
- Redis
- API-based service communication
- Local development and deployment workflow

---

## Architecture Highlights

- Modular ERP/WMS architecture
- Separation between frontend, backend, database, and processing services
- Inventory changes controlled through backend business logic
- PostgreSQL as the source of truth for operational records
- Prisma-based schema and migration management
- Python processing services for Excel and file workflows
- REST API communication between frontend and backend
- Permission-aware workflow design
- Barcode-centered traceability model
- Scalable structure for future warehouse, shipping, and reporting expansion

---

## Business Workflow Concept

The system is designed around real operational flows such as:

```text
Sales Order
→ Fulfillment / Packing
→ Pallet / Container Allocation
→ Packing List
→ Shipment / Delivery Tracking
