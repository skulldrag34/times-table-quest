# Times Table Quest

Short daily games for practicing the 6s, 7s, 8s and 9s times tables. Runs in any browser, installs to the Home Screen, and works offline.

- Five games: Unicorn Quiz, Card War, Spinner Spin, Mystery Number, Find My Gaps
- Starts untimed and tap-to-answer. Typing and a 10s or 5s timer are switches in Settings
- Progress saves on the device. Settings has a backup code to move or restore it
- No accounts, no ads, no tracking, no network calls except loading Google Fonts

## Run locally

Open `index.html` in a browser. For the offline feature to register, serve the folder instead:

```
python3 -m http.server 8080
```

## Publish with GitHub Pages

1. Push this folder to a GitHub repo (public repos work on free accounts).
2. Repo **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch **main**, Folder **/ (root)**, then Save.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Updating

Edit the files, commit, and push. Bump `CACHE` in `sw.js` (for example `ttq-v2`) so installed copies pick up the change. Devices refresh after the app is opened twice.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML, CSS, JS) |
| `manifest.webmanifest` | Install name, colors and icons |
| `sw.js` | Offline support |
| `icons/` | App icons |
