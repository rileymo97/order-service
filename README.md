# Order Service

A Node.js/Express microservice that handles order creation and management.

## Overview

This service is responsible for all order-related operations in the ecommerce platform. It communicates with the `product-service` to verify products exist before creating orders.

## API Endpoints

- GET    /health        - Health check
- GET    /orders        - Fetch all orders
- POST   /orders        - Create a new order
- PATCH  /orders/:id    - Update order status

## Prerequisites

- Node.js v25.6.0 (see `.nvmrc`)
- npm (comes with Node.js)
- PostgreSQL database running
- product-service running on port 3001

## Getting Started

1. Clone the repository
   git clone git@github.com:rileymo97/order-service.git

2. Install dependencies
   npm install

3. Set up environment variables
   cp .env.example .env
   Then open .env and fill in the required values

4. Start the service
   npm start

## Project Structure

order-service/
├── src/          # Application source code
├── tests/        # Test files
├── .env.example  # Environment variable template
├── .nvmrc        # Node.js version specification
└── index.js      # Application entry point

## Related Services
- ecommerce-frontend: https://github.com/rileymo97/ecommerce-frontend
- product-service: https://github.com/rileymo97/product-service
- database: https://github.com/rileymo97/database
