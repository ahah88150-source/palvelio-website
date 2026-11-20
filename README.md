# Palvelio

A responsive, multilingual home services website for Helsinki, Espoo and Vantaa. Customers can request home cleaning, moving help, furniture assembly and small repairs. Providers have a dedicated introduction and application flow.

Built with React 19, TypeScript, TanStack Start, Vite and Netlify Forms. English, Finnish and Arabic copy is maintained in `src/components/MarketingPage.tsx`; Arabic uses right-to-left layout. Language preference is saved in the browser. Enquiries are stored by Netlify Forms, with no application database or credentials required.

## Local development

Use Node 22.13+ or Node 24 and pnpm. Install with `pnpm install`, then use `pnpm dev`. To emulate Netlify, run `netlify dev --port 8889`. Form processing requires a Netlify deployment; a plain local preview cannot deliver submissions.

## Configuration

Brand metadata lives in `src/data/site.ts`, shared layout in `src/routes/__root.tsx`, and responsive styles in `src/styles.css`. Photography is served from Unsplash and fonts from Google Fonts. No payments or instant bookings are offered. Enquiries and provider applications are distinguished by the `role` field in the `palvelio-enquiries` Netlify form. Service IDs 0–3 map to cleaning, moving, assembly and repairs respectively. Review submissions in the site's Netlify Forms dashboard.
