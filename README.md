# Interlink

Static interlinking and article-host source repository.

This repo is structured so the same content can be connected to multiple static hosts:

- Netlify
- Vercel
- Render Static Sites
- GitHub Pages
- Cloudflare Pages
- Surge-style static deployments

## Structure

```text
sites/
  netlify/
  vercel/
  render/
  github-pages/
  cloudflare-pages/
  surge/
shared/
  assets/
  css/
```

Each provider folder can be used as a site root, or the full repository can be deployed as one multi-folder static site.

## Article pattern

Each article/page should usually live at:

```text
sites/<provider>/<slug>/index.html
sites/<provider>/<slug>/hero.webp
```

That creates clean URLs like:

```text
https://example-host.com/<slug>/
```

No production articles are included yet. This is just the publishing scaffold.
