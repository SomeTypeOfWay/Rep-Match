# Rep Match

Pick the muscles you want to train and the gear you have, match a workout style, set your time, and go.

- 254 exercises, 16 warm-ups and 20 stretches, each with an animated keyframe demo and numbered steps
- 11 workout styles: Classic Build, Heavy 5×5, Superset Pairs, Giant Sets, Circuit, EMOM, AMRAP, Tabata, Pyramid, High-Rep Burn, Slow Tempo
- Plans fill the time you set, warm-up and cool-down included
- Guided player with timers, beeps and a screen wake lock
- Works offline once it has been opened, and installs to the iPhone Home Screen

Everything runs in the browser. Your picks, skipped exercises and workout history are saved on your device only (browser local storage). Nothing is sent anywhere.

## Put it on GitHub Pages

1. Create a new repository on GitHub, for example `rep-match`. It can be public, or private if your plan includes Pages for private repos.
2. Upload everything in this folder to the root of the repository: `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, `README.md` and the `icons` folder. On github.com use **Add file → Upload files** and drag the files and the `icons` folder in, then **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, pick **main** and **/ (root)**, and save.
4. After a minute or two the site is live at `https://<your-username>.github.io/rep-match/`.

## Add it to your iPhone Home Screen

Open the site in Safari, tap **Share**, then **Add to Home Screen**. It opens full screen like an app, with its own icon.

## Updating

Replace `index.html` and `sw.js` with the new versions and commit. The app checks for the new version when it opens with a connection. If you still see the old version, close it and open it again.

## Files

| File | What it does |
| --- | --- |
| `index.html` | The whole app: layout, exercise library, pose engine and player |
| `manifest.webmanifest` | App name, icons and full-screen mode for the Home Screen |
| `sw.js` | Service worker that caches the app so it works offline |
| `icons/` | Home Screen, browser and favicon icons |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

Fonts (Big Shoulders Display and Barlow) load from Google Fonts and are cached for offline use.
