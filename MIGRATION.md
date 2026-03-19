# Migration checklist — do this before deleting the source site

Complete every step below so this repo has **all** assets locally. No content should depend on the Google site or Drive after you delete it.

---

## 1. Images (13 files)

### Artwork — 5 images

1. Open https://sites.google.com/site/nologygames/artwork
2. Right‑click each image → **Save image as…**
3. Save into the `images/` folder in this repo with these **exact** names:
   - `artwork-1.jpg` (first image)
   - `artwork-2.jpg`
   - `artwork-3.jpg`
   - `artwork-4.jpg`
   - `artwork-5.jpg` (fifth image)

### Team — 8 images

1. Open https://sites.google.com/site/nologygames/team
2. Right‑click each image → **Save image as…**
3. Save into the `images/` folder with these **exact** names:
   - `team-1.jpg` … `team-8.jpg` (in order)

---

## 2. Game installers — 6 files

1. Open https://drive.google.com/folderview?id=1wpGTQimegcQ3Xk0AjDq6h9TPf8anCggj
2. Download each file into the `downloads/` folder. Use the `Nology-` prefix when saving:
   - `Nology-ChipSSetup.exe` (from ChipSSetup.zip or installer)
   - `Nology-CookieChefSetup.exe`
   - `Nology-HelloSetup.exe`
   - `Nology-JoKenPoSetup.exe`
   - `Nology-KokoArenaSetup.exe`
   - `Nology-SPMSetup.exe`

---

## 3. Verify

- [ ] `images/` contains 13 files: `artwork-1.jpg` … `artwork-5.jpg`, `team-1.jpg` … `team-8.jpg`
- [ ] `downloads/` contains 6 installer files (Nology-*.exe)
- [ ] Open `index.html` (or run a local server) and check:
  - [ ] [Artwork](artwork.html) — all 5 images load
  - [ ] [Team](team.html) — all 8 images load
  - [ ] [Downloads](downloads.html) — each link downloads the correct file

After this, you can safely delete the Google site and, if desired, the Drive folder. The repo is self‑contained.
