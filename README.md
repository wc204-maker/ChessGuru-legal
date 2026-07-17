# Chess Second — legal pages (public)

Static privacy policy and terms for App Store Connect. **No app source code** — safe to publish as a public repo.

## Live URLs (after GitHub Pages is enabled)

- Privacy: `https://wc204-maker.github.io/chess-second-legal/privacy.html`
- Terms: `https://wc204-maker.github.io/chess-second-legal/terms.html`

## One-time setup

Run these in Terminal from this folder:

```bash
cd "/Users/willsaccount/Developer/Coding Apps/Chess/ChessGuru/chess-second-legal"
git init
git add .
git commit -m "Add Chess Second privacy policy and terms"
gh repo create chess-second-legal --public --source=. --push
```

Then on GitHub:

1. Open **https://github.com/wc204-maker/chess-second-legal**
2. **Settings** → **Pages**
3. **Build and deployment** → Source: **Deploy from a branch**
4. Branch: **main** → folder **/ (root)** → **Save**
5. Wait ~2 minutes, open the privacy URL above in Safari

Paste the privacy URL into **App Store Connect** → **Chess Second** → **App Information** → **Privacy Policy URL**.
