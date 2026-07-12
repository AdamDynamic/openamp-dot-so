# Open Amplitude Society

> An open catalogue of music hardware you can build yourself.

The source for the Open Amplitude Society website — a static
[Hugo](https://gohugo.io) site with no framework, one hand-written stylesheet,
and near-zero JavaScript. It's deployed on Netlify straight from this
repository (`netlify.toml`).

## Run it locally

You need **Hugo extended** — the exact version is pinned in `netlify.toml`
(`HUGO_VERSION`). Then, from this directory:

```bash
hugo server
```

and open the URL it prints (<http://localhost:1313>).

## Build

```bash
hugo --gc --minify
```

The static site is written to `public/`. Netlify runs this on every push.

## Structure

| Path | What's there |
|------|--------------|
| `content/` | The catalogue entries (`catalogue/opamp-NNNN.md`) and pages, in Markdown |
| `layouts/` | Hand-written templates (no theme) |
| `assets/` | The single stylesheet (fingerprinted through Hugo Pipes) and images |
| `static/`, `data/` | Static files and structured data (categories, builds) |
| `netlify.toml` | Build command, publish dir, and security headers |

## Credits

Image attributions are in [`CREDITS.md`](CREDITS.md).
