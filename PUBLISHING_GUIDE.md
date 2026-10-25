# Publishing Guide — Crumb Cafe OS Portfolio Repository

## Repository strategy

Create a **new public repository** such as `crumb-cafe-os-portfolio`. Keep the actual application source in a separate private repository.

This kit contains only Markdown documentation and a `.gitignore`; it does not contain the application source or database dump.

## Suggested repository structure

```text
crumb-cafe-os-portfolio/
├── README.md
├── PUBLISHING_GUIDE.md
└── docs/
    ├── PRODUCT_OVERVIEW.md
    ├── FEATURES.md
    ├── TECHNICAL_OVERVIEW.md
    ├── SECURITY_AND_SCOPE.md
    └── screenshots/
        └── README.md
```

After capturing genuine screenshots, place them in `docs/screenshots/` and update the root README.

## Publish with Git

1. Create an empty public repository on GitHub. Do not initialize it with a README if you plan to push this folder directly.
2. Extract this kit and open a terminal in the extracted folder.
3. Run:

```bash
git init
git add README.md PUBLISHING_GUIDE.md docs .gitignore
git status
git commit -m "Add Crumb Cafe OS product documentation"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

Replace the remote URL with your real repository URL.

## Before pushing

- Confirm the folder contains only approved documentation and genuine screenshots.
- Do not copy `crumb(6).zip`, `.env`, `laravel.log`, or `theabacu_crumb(1).sql` into this repository.
- If the application source or secrets were previously committed to any public Git repository, deleting the file in a later commit is not enough: rotate secrets and review/clean Git history.
- Confirm screenshot data is synthetic and does not expose private customer information.
- Verify every README link after publishing.

## Making the portfolio compelling

- Put the live application link near the top of the README.
- Add 5–8 real screenshots that show meaningful workflows, not just the landing page.
- Keep feature claims aligned with the live version.
- Link the documentation files near the top so visitors can explore the product architecture and scope quickly.
- State clearly that the source code is private and this repository is a product case study, not an open-source release.
