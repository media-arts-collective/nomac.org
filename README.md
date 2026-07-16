# nomac.org

Source for the [Media Arts Collective](https://nomac.org) website — a small
volunteer-driven 501(c)(3) nonprofit based in New Orleans, Louisiana,
supporting community-based creative technology, public art, and media
projects (e.g. the "Supernova" light installation, a mobile "Projection
Car," and a bicycle-powered "Bike Sound System").

## What this is

A single static page (`index.html` + `style.css`) with:

- A hero header with the org wordmark, tagline, a Stripe donation link, and
  a "Get Involved" mailto CTA.
- **Current Projects** — Supernova, Projection Car, Bike Sound System.
- **About Us** — org history/mission blurb.
- **Team** — staff cards (Zachary Pine, Alexander Herzog, Brandon Bales)
  with circular avatar photos.
- **Board of Directors** — officer list.
- **Partners** — Cinema Sanctuary, Lafitte Greenway Partnership, Krewe de
  Vélorévolte, Virtual Krewe of Vaporwave.
- **Contact** — mailto link (info@nomac.org).

No build step, framework, or JS — plain HTML/CSS meant to be served as-is.

## Deployment

The `CNAME` file (containing `nomac.org`) is a GitHub Pages custom-domain
marker: this repo is served directly via GitHub Pages, with `nomac.org`
pointed at it via DNS. Pushing to `main` is the deploy step — there is no
separate build/publish pipeline.

## File layout

| Path          | Purpose                                          |
|---------------|---------------------------------------------------|
| `index.html`  | Page markup/content                               |
| `style.css`   | All page styling                                  |
| `CNAME`       | GitHub Pages custom domain (`nomac.org`)          |
| `hero.jpg`    | Hero header background image                      |
| `Zach.png`    | Team avatar — Zachary Pine (President)            |
| `Alex.png`    | Team avatar — Alexander Herzog (Client Relationship Manager) |
| `Brandon.png` | Team avatar — Brandon Bales (Communications Director) |

## Repo notes

This folder is its own git repository (remote:
`git@github.com:media-arts-collective/nomac.org.git`), independent of the
parent `vkv` monorepo it happens to live inside on disk.
