# Fabell

Static HTML storefront and admin dashboard.

- `index.html` — storefront
- `admin.html` — admin dashboard, served at `/admin.html`
- `config.js` — public Supabase project URL and publishable key
- `netlify.toml` — static hosting configuration

## Deploy
Import this repository into Netlify and publish the repository root (no build command required). Future commits to `main` will redeploy automatically once Git-based deployment is connected.

## Important
The Supabase browser key is a publishable key, not a service-role secret. Database security relies on Row Level Security. Before taking real orders, verify the checkout flow and reconcile the order-validation trigger with the live catalog fields (`title`/`price` versus legacy `n`/`p`).
