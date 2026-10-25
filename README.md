<div align="center">

# ☕ Crumb Cafe OS

### A multi-tenant cafe website and point-of-sale platform

**Run the counter. Manage the menu. Track orders and expenses. Understand your cafe — in one workspace.**

[![Live Application](https://img.shields.io/badge/Live%20Application-Visit%20Crumb-ef8b52?style=for-the-badge)](https://crumb.theabacuses.com/)
[![Product Docs](https://img.shields.io/badge/Documentation-Explore%20the%20Project-24352c?style=for-the-badge)](docs/PRODUCT_OVERVIEW.md)

[Product Overview](docs/PRODUCT_OVERVIEW.md) · [Feature Guide](docs/FEATURES.md) · [Technical Overview](docs/TECHNICAL_OVERVIEW.md) · [Security & Scope](docs/SECURITY_AND_SCOPE.md) · [Screenshot Guide](docs/screenshots/README.md)

</div>

---

## ✨ At a glance

Crumb Cafe OS is a SaaS-style operations platform designed for independent cafes. It brings together a cafe workspace, public menu/storefront, point-of-sale workflow, order management, customer records, expenses, and reporting.

<details open>
<summary><strong>🚀 Try the live product</strong></summary>

**[Open Crumb Cafe OS →](https://crumb.theabacuses.com/)**

Explore the public-facing experience. If registration is enabled, create a test workspace with your own email and synthetic data. Avoid entering real customer or payment information in a demo environment.
</details>

## 📸 Product screenshots

Screenshots are one of the most important parts of this portfolio. The supplied source ZIP did not contain screenshot images, and the live site could not be fetched by the review environment. To avoid presenting fabricated images as real product evidence, add genuine screenshots captured from your running application to the paths below.

| Product area | Screenshot file | What to show |
|---|---|---|
| Public landing page | `docs/screenshots/cafe-landing.png` | Crumb brand, value proposition, and sign-up CTA |
| Overview dashboard | `docs/screenshots/dashboard.png` | Sales, orders, customers, expenses, recent orders |
| POS checkout | `docs/screenshots/pos-checkout.png` | Menu items, cart, payment method, total |
| Menu management | `docs/screenshots/menu-management.png` | Categories, items, prices, availability |
| Order management | `docs/screenshots/order-management.png` | Order list, status, totals, channels |
| Reports | `docs/screenshots/reports.png` | Date range, sales/expense summary, ledger |
| Cafe storefront | `docs/screenshots/cafe-storefront.png` | Public cafe menu and order form |
| Mobile experience | `docs/screenshots/mobile-experience.png` | A key workflow at a mobile viewport |

See the [screenshot capture checklist](docs/screenshots/README.md) for details. Once you add the files, replace this table with an image gallery so visitors can see the product directly from GitHub.

## 🧩 What Crumb helps a cafe do

<details open>
<summary><strong>🧾 Point of sale</strong></summary>

Build a cart, calculate a sale, capture order details, and associate order items with the relevant cafe workspace.
</details>

<details open>
<summary><strong>🍽️ Menu and categories</strong></summary>

Organize menu categories and items, maintain prices and availability, and keep the cafe's storefront menu aligned with its records.
</details>

<details open>
<summary><strong>🌐 Cafe storefront and website orders</strong></summary>

Provide a cafe-specific public storefront where customers can browse available items and submit order requests for staff to review.
</details>

<details open>
<summary><strong>📦 Order management</strong></summary>

Review orders, inspect line items and customer information, and update order details and status.
</details>

<details open>
<summary><strong>👥 Customer records</strong></summary>

Keep customer contact records and associate customers with relevant orders.
</details>

<details open>
<summary><strong>💸 Expense tracking</strong></summary>

Record operating expenses with categories, amounts, dates, and optional notes.
</details>

<details open>
<summary><strong>📊 Reports and business visibility</strong></summary>

Use date-filtered reporting to review sales, expenses, item performance, and order/expense ledgers. The supplied update notes also describe print-friendly report output.
</details>

<details open>
<summary><strong>⚙️ Cafe settings and responsive experience</strong></summary>

Maintain cafe profile details such as its name, tagline, phone, and address. The source includes responsive styling and a PWA-oriented manifest/service-worker shell.
</details>

Feature details and current boundaries: [Feature Guide](docs/FEATURES.md).

## 🛠️ Technical snapshot

| Area | Implementation |
|---|---|
| Backend framework | Laravel 12 |
| Language | PHP 8.2+ |
| UI | Blade templates, CSS, vanilla JavaScript |
| Database access | Laravel Query Builder (`DB::table`); no Eloquent models in the reviewed controller |
| Database | MySQL / MariaDB |
| Product structure | Organization-scoped cafe workspaces |
| Deployment context | Shared-hosting-oriented setup documented in the supplied project files |

Explore the [Technical Overview](docs/TECHNICAL_OVERVIEW.md) for the request flow, main data entities, and architecture notes.

## 🧭 Explore Crumb

1. **[Open the live application](https://crumb.theabacuses.com/).**
2. Review the public landing page and cafe storefront experience.
3. If registration is enabled, create a test workspace with non-sensitive test data.
4. Explore the POS, menu, orders, customers, expenses, reports, and settings available to your account.
5. Read the project docs to understand feature scope, technical choices, and release-readiness considerations.

Individual routes and features may depend on the current deployment and the account used.

## 📚 Project documentation

- **[Product Overview](docs/PRODUCT_OVERVIEW.md)** — problem, intended users, and core workflow.
- **[Feature Guide](docs/FEATURES.md)** — capabilities and user journeys.
- **[Technical Overview](docs/TECHNICAL_OVERVIEW.md)** — stack, high-level architecture, and data entities.
- **[Security & Scope](docs/SECURITY_AND_SCOPE.md)** — review boundaries, known limitations, and hardening checklist.
- **[Screenshot Guide](docs/screenshots/README.md)** — recommended screenshot set and privacy-safe capture guidance.
- **[Publishing Guide](PUBLISHING_GUIDE.md)** — how to publish this portfolio kit without exposing the app source.

## 🔒 Source code and intellectual property

This is a **public product case study and documentation showcase**. The application source code is maintained privately and is not licensed for public reuse through this repository. Documentation and approved screenshots demonstrate product thinking, implementation scope, and engineering decisions.

This is **not an open-source release**. No permission is granted to copy, redistribute, or commercially use the private application source.

## ⚠️ Honest scope and limitations

Crumb Cafe OS is an evolving product. Based on the supplied source package and project notes:

- The storefront submits order requests; the reviewed code does **not** configure an online card-payment gateway.
- An order's payment method or status is an operational record, not proof that a card transaction was processed.
- The schema supports organization-scoped records and many controller operations apply organization filters; this does not constitute an independent tenant-isolation audit.
- Automated tests, authorization/tenant-isolation testing, backup/restore verification, and production security review should be completed before a commercial launch.
- The live application could not be independently fetched during preparation, so verify screenshots and live behavior against the current deployment before publishing claims.

Read [Security & Scope](docs/SECURITY_AND_SCOPE.md) for the complete checklist.

---

<div align="center">

**Built to simplify everyday cafe operations.**

[☕ Visit Crumb Cafe OS](https://crumb.theabacuses.com/)

</div>
