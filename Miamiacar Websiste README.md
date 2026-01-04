# Miamiacar.com – Polished Website (Next.js + Tailwind + PWA)

Company: **Miamiacar Inc**
Support: **support@miamiacar.com**
Launch: **March 10, 2026**

Included:
- SEO-ready copy across 34+ pages (per-page Metadata)
- Tailwind styling + subtle animations
- GDPR-friendly cookie consent + conditional analytics (Plausible/GA4)
- Newsletter hook for Mailchimp (Brevo-ready via backend)
- Media Kit downloads (PDF + logo SVGs)
- PWA support (manifest + service worker + icons)
- Static export deployable to Cloudflare Pages/Netlify/Vercel
- Optional admin CMS via Decap at `/admin/`

## Run
```bash
npm install
npm run dev
```

## Build static export
```bash
npm run build
```
Output: `out/`

## Analytics (GDPR-safe)
Analytics only loads after user clicks **Accept analytics**.
Set one:
- `NEXT_PUBLIC_PLAUSIBLE_DOMAIN=miamiacar.com`
- or `NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX`

## Newsletter
Set `NEXT_PUBLIC_MAILCHIMP_ACTION` to your Mailchimp subscribe POST URL.
For Brevo, route subscriptions via your backend API and update `components/NewsletterForm.tsx`.

## Deploy (Cloudflare Pages)
Build command: `npm run build`
Output directory: `out`
