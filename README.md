# mantisxgato-site

Företagssida för Mantis × Gato, byggd med [Astro](https://astro.build) och publicerad på GitHub Pages.

## Utveckling

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # bygger till ./dist
```

## Struktur

- `src/pages/index.astro` – startsidan (allt innehåll)
- `src/config.ts` – namn, domän, e-post
- `src/styles/global.css` – färger och typografi
- `.github/workflows/deploy.yml` – bygger och publicerar vid push till `main`

## Publicering

1. GitHub → Settings → Pages → Source: **GitHub Actions**.
2. Lägg den egna domänen i `public/CNAME` och i `astro.config.mjs` (`site`).
3. Peka DNS mot GitHub Pages och slå på **Enforce HTTPS**.
