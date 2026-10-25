# Screenshot Checklist

This folder is intended for **real screenshots captured from Crumb Cafe OS**. No screenshots are included yet because the live site could not be fetched by the review environment, and generated mockups should not be presented as real product evidence.

## Recommended captures

Save PNG or WebP files using these exact names so the root README links can be updated easily:

1. `dashboard.png` — cafe overview dashboard with synthetic data.
2. `pos-checkout.png` — POS screen with sample menu items and a populated cart.
3. `menu-management.png` — menu categories and items.
4. `order-management.png` — order list or order detail, with personal data hidden.
5. `customers-expenses.png` — customer list or expense management screen using test data.
6. `reports.png` — report date range and summary/ledger.
7. `cafe-storefront.png` — public cafe storefront with sample menu.
8. `mobile-experience.png` — mobile viewport showing a key workflow.

## Capture checklist

- Use a dedicated demo/test workspace and synthetic names, phone numbers, and orders.
- Do not show real customer data, real emails, passwords, session cookies, payment information, or admin secrets.
- Capture the browser viewport cleanly; hide bookmarks and unrelated tabs.
- Prefer consistent browser width and crop each image to the relevant interface.
- Use a clear, descriptive alt text when embedding images in Markdown.
- Confirm the live site still displays the feature before capturing it.

## Embed a screenshot in Markdown

```md
![Crumb Cafe OS dashboard](docs/screenshots/dashboard.png)
```

The root README currently documents expected filenames. Once the screenshots exist, replace the placeholder table with a gallery using the real images.
