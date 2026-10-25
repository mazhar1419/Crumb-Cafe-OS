# Technical Overview

## Stack

- **PHP:** `^8.2`
- **Framework:** Laravel `^12.0`
- **Presentation:** Blade templates, CSS, vanilla JavaScript
- **Database:** MySQL 8+ or MariaDB 10.5+ according to the supplied project README
- **Database access:** Laravel Query Builder; the reviewed application controller uses `DB::table` rather than Eloquent models
- **Hosting model:** project documentation discusses deployment on shared hosting / cPanel

## High-level request flow

1. A browser requests a public page, storefront, or authenticated workspace route.
2. Laravel routes the request to the cafe controller.
3. For authenticated workspace actions, the controller checks the session and active organization.
4. The controller reads or writes organization-scoped records through the query builder.
5. Blade templates render the interface; JavaScript handles client-side interactions.

## Main data entities

The supplied schema defines eight core application tables:

- `organizations` — cafe/workspace identity and status.
- `users` — owner/user accounts associated with an organization.
- `menu_categories` — cafe-specific menu categories.
- `menu_items` — products/menu items associated with a cafe and category.
- `customers` — customer contact records scoped to a cafe.
- `orders` — order headers, status, totals, and payment metadata.
- `order_items` — line items belonging to an order.
- `expenses` — cafe expense records.

The schema uses organization IDs and foreign-key relationships for core data ownership. This is a description of the supplied schema, not an independent proof that every route is secure against cross-tenant access.

## Transaction handling

The reviewed controller uses database transactions for website order creation and POS sale creation. Input validation is applied to registration, authentication, order submission, POS, menu, expense, and settings workflows. Some routes have request throttling.

## Routes and application areas

The supplied `routes/web.php` includes public landing/storefront routes, registration/login/logout, dashboard, POS, menu categories/items, customers, orders, expenses, reports, and settings.

## Deployment configuration

The supplied project README and checklist describe:
- Configure a production `.env` with `APP_DEBUG=false`, a valid `APP_KEY`, database credentials, and application URL.
- Enable required PHP extensions including `mbstring` and `pdo_mysql`.
- Ensure Laravel storage and cache directories are writable.
- Use HTTPS.
- Import the schema through a controlled setup process, then remove or disable the one-time database-install route.

**Never publish `.env`, production SQL exports, application logs, real customer data, or private source files in the public portfolio repository.**
