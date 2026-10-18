# Requirement Traceability — KKNUV

Statuses distinguish code presence from runtime verification. `IMPLEMENTED — NOT TESTED` means implementation is present but has not been verified in a running browser/build.

| ID | Requirement | Implementation location | Status | Test procedure / limitation |
|---|---|---|---|---|
| R-01 | Preserve supplied project, assets and configuration | `source/`, `public/`, `package.json`, `vite.config.js`, `vercel.json` | IMPLEMENTED — NOT TESTED | Compare archive file inventory; source derived from latest supplied ZIP |
| R-02 | Sticky responsive navigation with company identity | `Header`, `Brand`, CSS | IMPLEMENTED — NOT TESTED | Test desktop dropdowns, mobile menu, keyboard and route changes |
| R-03 | Products, services and academic navigation | `Header`, `ProductsPage`, `Services`, `AcademicProjectsPage` | IMPLEMENTED — NOT TESTED | Visit all menu links and refresh direct routes |
| R-04 | Exact hero message and supporting copy | `Home` | IMPLEMENTED — NOT TESTED | Compare displayed content with master prompt |
| R-05 | Floating assistant with eight suggested questions | `FloatingAssistant` | IMPLEMENTED — NOT TESTED | Click each prompt; responses are scripted, not live AI |
| R-06 | Trust strip with seven capability labels | `Home` trust-strip section | IMPLEMENTED — NOT TESTED | Verify all labels and responsive wrapping |
| R-07 | Products showcase and NexoraHub | `Home`, `ProductsPage`, `ProductDetail` | ACCEPTED EXCEPTION — DOCUMENTED | Concept placeholder only; real product facts/status not supplied |
| R-08 | Services overview and detail routes | `services`, `allServices`, `Services`, `ServiceRouter` | IMPLEMENTED — NOT TESTED | Check service cards, direct route and unknown slug handling |
| R-09 | Academic projects, B.Tech and M.Tech page families | `AcademicProjectsPage`, route map | IMPLEMENTED — NOT TESTED | Open all three routes and contact links |
| R-10 | Six Why NuvoraMind value blocks | `Home` section `#why-nuvora` | IMPLEMENTED — NOT TESTED | Confirm six blocks and order |
| R-11 | Technology ecosystem with 13 labels | `Home` section `#technology-ecosystem` | IMPLEMENTED — NOT TESTED | Confirm React, Node.js, Express, MongoDB, Python, Java, AI, ML, Cloud, AWS, Docker, Git and Figma |
| R-12 | Six-stage process in exact order | `ProcessTimeline`, `stages`, `Home` | IMPLEMENTED — NOT TESTED | Click each stage; reduced-motion behavior; process page |
| R-13 | Three pricing plans and Business Most Popular | Homepage pricing and `/pricing` | IMPLEMENTED — NOT TESTED | Verify Starter ₹4,999, Business ₹12,999, Professional ₹19,999 and Choose Plan links; confirm commercial terms before launch |
| R-14 | Custom solutions section | `Home` section `#custom-solutions` | IMPLEMENTED — NOT TESTED | Check CTA route and mobile stacking |
| R-15 | Portfolio labelled concept/demo | `ProjectCard`, `Projects`, homepage portfolio | IMPLEMENTED — NOT TESTED | Confirm labels and no fabricated client claims |
| R-16 | Honest testimonials placeholder | `Home` section `#testimonials` | IMPLEMENTED — NOT TESTED | Confirm placeholder is not presented as genuine customer quote |
| R-17 | Final CTA and FAQ | `CTA`, `HomeFAQ`, `FAQ` | IMPLEMENTED — NOT TESTED | Click CTA and test accordion keyboard states |
| R-18 | Contact fields, validation and honest submission state | `Contact` | IMPLEMENTED — NOT TESTED | Validate required fields; email app opens via mailto; no backend delivery claimed |
| R-19 | Footer groups and legal pages | `Footer`, `Legal` | IMPLEMENTED — NOT TESTED | Follow each link; legal copy is draft, not legal approval |
| R-20 | Light/dark theme and professional typography | `aurora-theme.css`, `App` | IMPLEMENTED — NOT TESTED | Toggle themes and inspect contrast at desktop/mobile widths |
| R-21 | Responsive layout, keyboard access and reduced motion | `aurora-theme.css`, semantic controls | IMPLEMENTED — NOT TESTED | Manual browser test still required; no responsive pass claimed |
| R-22 | SEO title, description and internal routes | `index.html`, `App`, `vercel.json` | IMPLEMENTED — NOT TESTED | Verify metadata, direct route refresh and deployment rewrite |
| R-23 | Install dependencies and production build | `package.json` | BLOCKED — DEPENDENCY | `npm install --no-audit --no-fund` timed out; `vite` unavailable, so `npm run build` could not run |
| R-24 | ZIP integrity and deliverable structure | `KKNUV.zip` | TESTED — PASS | `unzip -t` completed without compressed-data errors; expected project and documentation files are present |

## Known exceptions

- The product feature list, NexoraHub availability and product integrations are not verified in source materials. A concept-only presentation is used.
- The testimonial area intentionally contains a placeholder because no approved customer testimonials were supplied.
- Contact uses `mailto:` only; authentication and assistant are demos.
- Google Fonts depend on network access, with system fallback fonts.
- Full runtime, browser, Lighthouse and viewport testing could not be performed because dependency installation timed out.
