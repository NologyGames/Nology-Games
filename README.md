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

**Use a local server** so images load correctly (some browsers block images when opening HTML via `file://`):

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## GitHub Pages

To publish: **Settings → Pages** → Source: deploy from branch → main (root). The site will be at `https://<user-or-org>.github.io/Nology-Games/`.

## Adding game installers

Place the 6 installer ZIPs in the `downloads/` folder. See [downloads/README.md](downloads/README.md) for the file list and source link.
