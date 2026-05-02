# BetchaBippy® Mind Games — PWA

## Files in this package
- `index.html` — The complete app (all 4 games)
- `manifest.json` — PWA manifest (name, icons, theme color)
- `sw.js` — Service worker (offline support, caching)
- `icons/icon-192.png` — App icon (home screen)
- `icons/icon-512.png` — App icon (splash screen)

---

## How to go live in 5 minutes (free)

### Option A — Netlify Drop (easiest, zero account required)
1. Go to https://app.netlify.com/drop
2. Drag the entire `betchabippy-pwa` folder onto the page
3. Netlify gives you a live HTTPS URL instantly (e.g. `https://random-name.netlify.app`)
4. Share that URL with friends — on mobile they'll see "Add to Home Screen"

### Option B — GitHub Pages (free, permanent URL)
1. Create a free account at https://github.com
2. Create a new repository called `betchabippy`
3. Upload all files from this folder
4. Go to Settings → Pages → set Source to "main branch"
5. Your app is live at `https://yourusername.github.io/betchabippy`

### Option C — Vercel (free, fastest CDN)
1. Go to https://vercel.com and sign up free
2. Install Vercel CLI: `npm i -g vercel`
3. From this folder run: `vercel`
4. Follow the prompts — live in under 1 minute

---

## How to install on iPhone
1. Open the live URL in Safari (must be Safari, not Chrome)
2. Tap the Share button (box with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Tap "Add" — BetchaBippy® appears on your home screen like a real app

## How to install on Android
1. Open the live URL in Chrome
2. Tap the three-dot menu
3. Tap "Add to Home Screen" or "Install app"
4. The install banner may also appear automatically

---

## Want a custom domain?
Buy `betchabippy.com` (or similar) at Namecheap or Google Domains (~$12/yr)
Then point it at your Netlify/Vercel/GitHub Pages URL — takes about 10 minutes.

---

## Next steps toward a real App Store app
1. Get the PWA working and tested with friends first
2. Install Capacitor: `npm install @capacitor/core @capacitor/cli`
3. Wrap this HTML app: `npx cap init && npx cap add ios && npx cap add android`
4. Build and submit to App Store / Google Play
   - Apple Developer account: $99/year
   - Google Play account: $25 one-time

## Notes
- The Wordsy AI scoring requires an internet connection (calls Anthropic API)
- All other games work fully offline once cached by the service worker
- Score sharing uses the native Web Share API on mobile (real share sheet!)
