# Subscription Management System (Brightloop Software)

An end-to-end subscription lifecycle platform inspired by Odoo Subscriptions: catalog setup, quotations, subscriptions, automatic recurring invoices, payment recording, and finance analytics dashboard.

## 5-Command Quick Start

```bash
# 1. Start PostgreSQL database
docker compose up -d

# 2. Setup backend environment and install dependencies
cd backend && cp .env.example .env && npm install

# 3. Run database migrations & seed demo data
npx prisma migrate dev --name init && npm run seed

# 4. Start backend API server (runs on http://localhost:5000)
npm run dev

# 5. In a new terminal, setup and run frontend (runs on http://localhost:3000)
cd ../frontend && cp .env.example .env.local && npm install && npm run dev
```

## Demo Credentials (Seeded)
- **Admin**: `admin@brightloop.test` / `Admin@1234`
- **Staff**: `staff1@brightloop.test` / `Staff@1234`
- **Customer**: `customer1@brightloop.test` / `Customer@1234`
