<div align="center">

# Crumb Cafe OS

### A multi-tenant cafe website and point-of-sale platform

**One workspace for cafe operations — from menu management to orders, expenses, and sales reporting.**

[**🚀 Open the Live Application**](https://crumb.theabacuses.com/)

[Product Overview](docs/PRODUCT_OVERVIEW.md) · [Feature Guide](docs/FEATURES.md) · [Technical Overview](docs/TECHNICAL_OVERVIEW.md) · [Security & Scope](docs/SECURITY_AND_SCOPE.md) · [Screenshots](docs/screenshots/README.md)

</div>

---

## Explore the product

Crumb Cafe OS is a SaaS-style operations platform designed to help independent cafes manage day-to-day workflows in one place. The application combines an owner workspace, a cafe storefront, point-of-sale workflows, order management, customer records, expense tracking, and reporting.

> **Try the product:** Open the live application and explore the public-facing experience. If you create an account, use your own details and avoid entering real customer or payment information in a demo environment.

[**Open Crumb Cafe OS →**](https://crumb.theabacuses.com/)

## Product screenshots

> Add genuine screenshots from the live application to the paths below before publishing. These are image placeholders, not screenshots of the current production site.

| Product area | Screenshot |
|---|---|
| Overview dashboard | `docs/screenshots/dashboard.png` |
| POS checkout | `docs/screenshots/pos-checkout.png` |
| Menu management | `docs/screenshots/menu-management.png` |
| Order management | `docs/screenshots/order-management.png` |
| Customers and expenses | `docs/screenshots/customers-expenses.png` |
| Reports | `docs/screenshots/reports.png` |
| Cafe storefront | `docs/screenshots/cafe-storefront.png` |
| Mobile experience | `docs/screenshots/mobile-experience.png` |

See the [screenshot checklist](docs/screenshots/README.md) for capture guidance.

## What it helps a cafe do

- **Run point-of-sale workflows:** build a cart, calculate a sale, record order details, and keep order items associated with the cafe.
- **Manage a menu:** organize categories and menu items, maintain prices and availability, and keep the storefront menu aligned with the cafe's records.
- **Receive website orders:** let customers submit an order request from a cafe-specific storefront; staff can review and update its status.
- **Keep customer records:** store customer contact details and associate them with orders.
- **Track operating expenses:** record expense categories, amounts, dates, and notes.
- **Review performance:** use date-filtered reporting to inspect sales, expenses, item performance, and order/expense ledgers.
- **Configure a cafe workspace:** maintain cafe profile details such as its name, tagline, contact details, and address.
- **Work across devices:** use a responsive interface with a PWA-oriented manifest/service-worker shell.

Feature details and current boundaries are documented in [Feature Guide](docs/FEATURES.md).

## Technical snapshot

| Area | Implementation |
|---|---|
| Backend framework | Laravel 12 |
| Language | PHP 8.2+ |
| UI | Blade templates, CSS, vanilla JavaScript |
| Database access | Laravel Query Builder (`DB::table`); no Eloquent models in the reviewed controller |
| Database | MySQL / MariaDB |
| Product structure | Organization-scoped cafe workspaces |
| Deployment context | Shared-hosting-oriented setup documented in the supplied project files |

See [Technical Overview](docs/TECHNICAL_OVERVIEW.md) for architecture and data boundaries.

## How to explore

1. Open the [live application](https://crumb.theabacuses.com/).
2. Review the public landing page and cafe storefront experience.
3. If registration is enabled, create a test workspace using your own email and non-sensitive test data.
4. Explore the POS, menu, orders, customers, expenses, reports, and settings areas available to your account.
5. Review the documentation in this repository for feature scope, technical choices, and known limitations.

Availability of individual routes and features depends on the current live deployment and the account you use.

## Documentation

- [Product Overview](docs/PRODUCT_OVERVIEW.md) — problem, intended users, and workflow.
- [Feature Guide](docs/FEATURES.md) — capabilities and user journeys.
- [Technical Overview](docs/TECHNICAL_OVERVIEW.md) — stack, application structure, and data model at a high level.
- [Security & Scope](docs/SECURITY_AND_SCOPE.md) — what is and is not claimed, plus pre-launch hardening items.
- [Screenshots](docs/screenshots/README.md) — capture checklist and expected filenames.

## Source code and intellectual property

This repository is a **public product case study and documentation showcase**. The application source code is maintained privately and is not licensed for public reuse through this repository. Public documentation and screenshots are provided to demonstrate product thinking, implementation scope, and engineering decisions.

Do not interpret this repository as an open-source release. No permission is granted to copy, redistribute, or commercially use the private application source.

## Honest scope notes

Crumb Cafe OS is an evolving product. In the reviewed source package:

- The website storefront submits order requests; the code does **not** configure an online card-payment gateway.
- A payment method or payment status stored against an order is an operational record, not proof of a card transaction.
- The reviewed schema supports organization-scoped records, and the controller uses organization filters in many operations; this documentation does not claim an independent tenant-isolation audit.
- The project notes identify automated tests, complete authorization/tenant-isolation testing, backup/restore procedures, and production security review as work that should be completed before a commercial launch.
- The live application could not be independently fetched during preparation of this kit, so screenshots and live behavior must be verified by the repository owner before publication.

See [Security & Scope](docs/SECURITY_AND_SCOPE.md) for details.

---

<div align="center">

**Built to simplify everyday cafe operations.**

[Open the Live Application](https://crumb.theabacuses.com/)

</div>
# Crumb-Cafe-OS
