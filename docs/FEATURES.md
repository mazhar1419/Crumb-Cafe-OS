# Feature Guide

This guide summarizes features visible in the supplied source package. The live deployment may differ; verify each area before using this document as a release checklist.

## 1. Cafe workspace and access

- Self-service cafe registration creates an organization/workspace and an owner user.
- The reviewed controller stores the organization ID and user ID in the session.
- Login checks the account and active organization; login attempts are rate-limited in the reviewed controller.
- Registration seeds starter menu categories and sample items.

**Scope note:** the supplied source does not show a full invitation-based team management or granular role-permission system. Do not advertise those capabilities without confirming the deployed version.

## 2. Public cafe storefront

- A cafe-specific URL is resolved from the cafe slug.
- Active categories and available menu items are shown.
- Customers can submit order details such as name, phone, location, order type, payment preference, and item quantities.
- The order request is associated with the relevant cafe organization.

## 3. Point of sale

- Staff can select available menu items and create a cart.
- Sale records are stored as orders with line items.
- The source includes validation and throttling for POS sale submission.
- Customer details can be associated with a sale when provided.

## 4. Menu management

- Create and edit categories.
- Create and edit menu items with category, description, price, and availability.
- Delete categories and items.
- List pages support pagination in the reviewed package.

## 5. Orders

- View order lists and order details.
- Review order items and customer information.
- Update order status.
- Edit order information including quantities, discount, order status, payment method/status, customer details, and notes, as described in the supplied update notes.

## 6. Customers

- Customer records can be created or updated through order workflows.
- Records are associated with a cafe organization.
- Customer list view supports pagination.

## 7. Expenses

- Record expense title, category, amount, date, and optional notes.
- Edit expense records.
- Review expenses and totals in the management interface.

## 8. Reports

The supplied update notes describe date-range reporting with:
- Daily order, sales, expense, and outcome summaries.
- Item-wise sales.
- Category filtering.
- Order and expense ledgers.
- Print-friendly report output.

## 9. Cafe settings

The settings workflow supports editing cafe profile fields such as name, tagline, phone, and address.

## 10. Responsive / PWA-oriented UI

The source package includes responsive CSS, a web app manifest, and a service-worker file. This supports a PWA-oriented shell, but should not be described as comprehensive offline POS operation unless that behavior has been tested and confirmed.

## Important payment distinction

The storefront offers payment preferences such as cash on delivery/pay at pickup and a card preference, but the reviewed source notes explicitly state that **no card gateway is configured**. Orders can be marked paid/unpaid by staff; this is an operational record and does not itself charge a card.
