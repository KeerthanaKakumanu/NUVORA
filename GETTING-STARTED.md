# Getting Started — KKNUV

## 1. Install dependencies

Use Node.js 20 or newer and npm. From the project root:

```bash
npm install
```

The current packaging environment timed out while retrieving npm dependencies, so `node_modules` and a generated lockfile are not included. If install fails on your machine, check network/proxy access and npm registry configuration.

## 2. Run development server

```bash
npm run dev
```

Vite is configured to bind to `0.0.0.0:3000` with a strict port. Visit the URL printed in the terminal.

## 3. Build and preview

```bash
npm run build
npm run preview
```

A production build was not verified in the packaging environment because Vite could not be installed after npm retrieval timed out. Do not deploy until a successful build and manual browser pass have been completed.

## 4. Routes

- `/`
- `/products`
- `/products/nexorahub` (concept placeholder)
- `/services` and `/services/:slug`
- `/academic-projects`
- `/btech-projects`
- `/mtech-projects`
- `/projects` and `/projects/:slug`
- `/process`
- `/pricing`
- `/about`
- `/contact`
- `/resources`
- `/privacy` and `/privacy-policy`
- `/terms` and `/terms-and-conditions`
- `/login` and `/signup` (demo only)
- unknown paths show a 404 page

`vercel.json` rewrites requests to `index.html` so client-side routes can be resolved by React Router.

## 5. Theme and branding

Use the header sun/moon control to switch themes. The refreshed interface uses near-black/navy surfaces in dark mode, white/soft-violet surfaces in light mode, violet `#6D28D9`, indigo `#4F46E5`, and readable neutral text. Inter is the primary font, with Manrope for display headings and system fallbacks.

## 6. Demo integrations and production checklist

- Assistant responses are scripted and must not be represented as live AI.
- Login/signup are not connected to authentication.
- Contact form uses `mailto:` and does not submit to a backend.
- Verify contact details and product facts before publishing.
- Confirm exact package inclusions and domain terms in writing.
- Test desktop, laptop, tablet and mobile widths, all menu states, form validation, route refresh and keyboard access.
