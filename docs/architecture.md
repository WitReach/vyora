# Vyora Architecture

Vyora follows a headless commerce architecture with a central control layer (OCC).

## Components

### Frontend (Next.js)

* Customer-facing storefront
* Fetches data via API
* Hosted on primary domain

### OCC (Operations Command Center - Laravel)

* Admin panel for managing products, orders, and users
* Page builder for dynamic storefront design
* Role-based access control
* Hosted on subdomain

## Integrations Layer

Vyora integrates with external services:

* WhatsApp Business (order notifications)
* Zoho (Books, Invoice, Campaigns)
* Email (SMTP / Zoho Mail)
* QikInk (POD dropshipping)

## Data Flow

Frontend → API (Laravel OCC) → External Services

This architecture allows flexibility, scalability, and modular development.
