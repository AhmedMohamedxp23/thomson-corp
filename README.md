# Thomson Corp — Multi-Region Corporate Site

Multi-locale (Malaysia / Singapore / China) corporate website with localized routing, product catalogue, and content pages (about, leadership team, careers, collaborations, loyalty, community, factory, blogs).

**Live:** [thomson-corp.vercel.app](https://thomson-corp.vercel.app)

## Tech Stack

Next.js 14 (App Router) · next-intl (i18n routing/middleware) · Tailwind CSS · GSAP (`@gsap/react`) · Swiper

## Structure

```
app/
  [locale]/            Locale-scoped routes: about-us, products, careers,
                        contact-us, leadership-team, collaborations, loyalty,
                        community, factory, blogs
  components/           Shared UI
  hooks/                 Custom hooks
i18n/
  routing.js            Locale routing config
  request.js
messages/
  cn.json, en-my.json, en-sg.json   Per-locale translation strings
middleware.js            next-intl middleware (matches "/" and locale-prefixed paths)
```

## Getting Started

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) — locale-prefixed routes are available at `/en-my` and `/en-sg`.

```bash
npm run build   # production build
npm run lint    # next lint
```
