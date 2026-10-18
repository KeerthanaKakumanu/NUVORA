# KKNUV — NuvoraMind website

A repaired, responsive React + Vite website project for NuvoraMind Pvt. Ltd. This package preserves the supplied React source, catalog data, deployment configuration and brand assets while refining the design system, navigation, homepage structure and required page families.

## Run locally

Requirements: Node.js 20+ and npm.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (the project configuration uses port `3000`). For a production build:

```bash
npm run build
npm run preview
```

## Key features

- Light/dark theme toggle with violet/indigo highlights and Inter/Manrope typography.
- Sticky responsive navigation with product, service and academic dropdowns.
- Homepage section order chosen for this repair: Hero → Trust strip → How we work → Technology ecosystem → Why NuvoraMind → Products → Services → Academic projects → Pricing → Custom solutions → Portfolio → Testimonials placeholder → Final CTA → FAQ → Contact.
- Required routes for products, service details, academic projects, B.Tech, M.Tech, portfolio, pricing, about, contact, privacy and terms.
- Concept previews clearly identify unverified product details and demo portfolio items.
- Scripted assistant, honest mailto enquiry form, interactive process timeline, FAQ and website estimator.
- Supplied identity assets retained; no invented client testimonials or product capabilities.

## Important limitations before production

- `npm install` could not complete in the packaging environment because dependency retrieval timed out; therefore a Vite production build and browser-based responsive tests could not be run here. Run the commands above on a connected machine and resolve any install/build errors before deployment.
- The assistant is scripted demo UI, not a connected AI service. Authentication/portal is a demo. The contact form prepares an email; it does not submit to a backend.
- NexoraHub product capabilities and status are not verified in the supplied materials. The product page is explicitly a concept placeholder.
- Pricing cards reflect the requested displayed package amounts. Package inclusions, free-domain terms, hosting, maintenance, taxes and revisions must be confirmed in writing before commercial use.
- Existing contact details were retained from the supplied source and should be verified by the owner before launch.
- Google Fonts are loaded remotely with local system fallbacks; if remote fonts are blocked, the site remains readable using fallback fonts.

See `GETTING-STARTED.md`, `ASSET-INVENTORY.md`, `IMPLEMENTATION-PLAN.md`, `REQUIREMENT-TRACEABILITY.md` and `FINAL-AUDIT-REPORT.md` for release details.
