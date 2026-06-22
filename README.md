# MyCafe

A native PHP cafe management system designed to streamline order management and operations for cafeteria services.

## Overview

MyCafe is a comprehensive web-based cafe management solution that enables efficient handling of cafe operations, including order placement, user management, product catalog management, and order tracking.

## Features

- **User Management**: Create and manage user accounts with role-based access (admin/user)
  - User profiles with email, password, room number, and extension
  - Security question and answer for account recovery
  - Admin dashboard for user administration

- **Product Catalog**: Manage products and categories
  - Organize products into categories (drinks, meals, cakes, pizza)
  - Track product availability and pricing
  - Product images and descriptions

- **Order Management**: Complete order lifecycle management
  - Create new orders with multiple products
  - Track order status (processing, out for delivery, done)
  - Add special notes to order items
  - Automatic order pricing calculation

- **Room Management**: Support for multi-room/multi-tenant environments
  - Assign orders to specific rooms
  - Room-based order tracking and delivery

- **Analytics & Reporting**: 
  - Date-range based order queries
  - Order summation and grouping capabilities
  - Order history and tracking

## Technology Stack

- **Language**: PHP (99%)
- **Database**: MySQL
- **Architecture**: ORM-based design pattern

## Database Schema

The system includes the following main tables:

- `users` - User accounts and profiles
- `products` - Product inventory
- `categories` - Product categories
- `orders` - Order records
- `order_product` - Order line items (many-to-many relationship)
- `rooms` - Room/location management

## ORM Implementation

MyCafe includes a custom ORM class (`database/model.php`) that provides:
- Database connection management
- CRUD operations (Create, Read, Update, Delete)
- Advanced query capabilities with WHERE conditions
- Date-range filtering
- Aggregation functions (sum, group by)
- Sorting and filtering

## Getting Started

1. Import the `database/cafeteria.sql` file into your MySQL database
2. Configure database connection in `appconf.php`
3. Access the web interface to manage cafe operations

## Use Cases

- Office/Corporate cafeteria operations
- Dorm/Hostel food delivery management
- Multi-room accommodation facility dining services
- Quick service restaurant order management
