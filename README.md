# Nology Games

Former game development company from Brazil. All games are free to download.

**Games:** [Koko Arena](game-koko-arena.html) · [JoKenPo](game-jokenpo.html) · [Cookie Chef](game-cookie-chef.html) · [Hello!](game-hello.html) · [Super Popcorn Machine](game-super-popcorn-machine.html) · [Chip$](game-chip.html)

**Book:** [Desenvolvimento de Jogos Eletrônicos - Teoria e Prática](http://www.novatec.com.br/livros/jogos2/) (Novatec Editora, 2005, Portuguese).

## Before you delete the source site

**Save all assets locally first.** This repo uses only local paths; nothing is hotlinked.

- **Images (13 files):** From the live site, save the 5 images on [Artwork](https://sites.google.com/site/nologygames/artwork) as `images/artwork-1.jpg` … `artwork-5.jpg`, and the 8 images on [Team](https://sites.google.com/site/nologygames/team) as `images/team-1.jpg` … `team-8.jpg`. See [images/README.md](images/README.md).
- **Game installers (6 files):** Download from the [Google Drive folder](https://drive.google.com/folderview?id=1wpGTQimegcQ3Xk0AjDq6h9TPf8anCggj) into `downloads/` with the `Nology-` prefix (e.g. `Nology-ChipSSetup.exe`). See [downloads/README.md](downloads/README.md).

Full checklist: [MIGRATION.md](MIGRATION.md).

## Run locally

The site uses **Jekyll** with the **[Slate](https://github.com/pages-themes/slate)** theme (`remote_theme: pages-themes/slate`) — dark header, light content band. Shared chrome is in [`_layouts/default.html`](_layouts/default.html) and [`_includes/`](_includes/). Overrides are in [`assets/nology-custom.css`](assets/nology-custom.css).

```bash
bundle install
bundle exec jekyll serve
```

Open **http://127.0.0.1:4000/Nology-Games/** (Jekyll serves under `baseurl`; there is nothing at `http://127.0.0.1:4000/book.html`). Example: **http://127.0.0.1:4000/Nology-Games/book.html**.

**If the page looks unstyled:** check DevTools → Network → `assets/css/style.css` and `nology-custom.css` (both **200**). Use `jekyll serve` at **`http://127.0.0.1:4000/Nology-Games/`** (`baseurl` in [`_config.yml`](_config.yml)).

To build static output only:

```bash
bundle exec jekyll build
python3 -m http.server 4001 --directory _site
# open http://localhost:4001/book.html
```

## GitHub Pages

**Settings → Pages** → deploy from branch **main** / **root**. GitHub will run Jekyll automatically. The site URL is `https://<user-or-org>.github.io/Nology-Games/` — relative `assets/` and `images/` links resolve under that path automatically.

## Adding game installers

Place the 6 installer ZIPs in the `downloads/` folder. See [downloads/README.md](downloads/README.md) for the file list and source link.
