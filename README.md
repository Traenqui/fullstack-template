# **PROJECT_NAME** – Fullstack Template

This repository is a reusable starter template for building products with:

- **Backend:** .NET (modular monolith, vertical slice)
- **Web:** React + Next.js
- **Mobile:** Expo (React Native)
- **Auth:** prepared for Keycloak (optional)

> This repo is meant to be used as a **GitHub Template Repository** and initialized via a script to rename identifiers and set project-specific configuration.

---

## Repository Structure

```txt
.
├── backend/        # .NET solution (Modular Monolith + Vertical Slice)
├── frontend/       # Next.js app
├── mobile/         # Expo app
├── scripts/        # initialization scripts (rename, token replacement)
├── .github/        # CI workflows (if any)
└── README.md

```

## Getting started

1. Create a new project from this template
   1. Click **Use this template** on GitHub
   2. Clone the new repository locally
   3. Run the initialization script to rename everything
1. Initialize (rename identifiers)
   From the repository root:

```sh
chmod +x ./scripts/init.sh
./scripts/init.sh \
  --name "__PROJECT_NAME__" \
  --slug "__PROJECT_SLUG__" \
  --ns "__PROJECT_NAMESPACE__" \
```

Arguments:
`--name` Human-readable product name (e.g. Acme Portal)
`--slug` Kebab-case slug (e.g. acme-portal)
`--ns` .NET namespace / solution prefix (PascalCase, e.g. AcmePortal)

After running the script, review the changes with git diff and commit.
