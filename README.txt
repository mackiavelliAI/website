# SaaS Landing Page (Static HTML + Tailwind CDN)

## Quick start (preview locally)
1. Download `index.html`.
2. Double‑click it to open in your browser (or run a tiny server: `python -m http.server 8080` and visit http://localhost:8080).

## Deploy options

### GitHub Pages (free)
1. Create a new GitHub repo and add `index.html`.
2. Settings → Pages → Set Source to **Deploy from a branch** (main / root).
3. Your site will be live at `https://<username>.github.io/<repo>`.

### Netlify (1‑click)
- Drag‑and‑drop the folder with `index.html` onto https://app.netlify.com/drop
- Or use CLI:
  ```
  npm i -g netlify-cli
  netlify deploy --prod
  ```
  When asked for the deploy folder, enter `.`

### Vercel (CLI)
```
npm i -g vercel
vercel --prod
```

## Custom domain
Point your domain’s DNS to your host (A/ALIAS for Netlify/Vercel, or CNAME for GitHub Pages). Add the domain in your host’s dashboard and finish verification.

## Customization
- Replace text, pricing, and testimonials in `index.html`.
- Swap the hero demo box with a screenshot/video embed.
- Update colors in the Tailwind config inline at the top (`brand`).

## Forms
This demo prevents actual submit. For a real inbox:
- **Formspree**: change `<form>` `action="https://formspree.io/f/XXXX"` and `method="POST"`.
- **Netlify Forms**: add `data-netlify="true"` to the `<form>` and include a `name` attribute.

## Next steps (optional, full stack)
- Convert to Next.js for routing, API routes, auth, and Stripe checkout.
