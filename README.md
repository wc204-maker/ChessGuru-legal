# ChessGuru — legal pages (public)

Static privacy policy and terms for App Store Connect. **No app source code** — safe to publish as a public repo.

## Live URLs (after GitHub Pages is enabled)

- Privacy: `https://wc204-maker.github.io/ChessGuru-legal/privacy.html`
- Terms: `https://wc204-maker.github.io/ChessGuru-legal/terms.html`
- Email verified: `https://wc204-maker.github.io/ChessGuru-legal/email-verified.html`

## One-time setup

Run these in Terminal from this folder:

```bash
cd "/Users/willsaccount/Developer/Coding Apps/Chess/ChessGuru/chessguru-legal"
git init
git add .
git commit -m "Add ChessGuru privacy policy and terms"
gh repo create chessguru-legal --public --source=. --push
```

Then on GitHub:

1. Open **https://github.com/wc204-maker/chessguru-legal**
2. **Settings** → **Pages**
3. **Build and deployment** → Source: **Deploy from a branch**
4. Branch: **main** → folder **/ (root)** → **Save**
5. Wait ~2 minutes, open the privacy URL above in Safari

Paste the privacy URL into **App Store Connect** → **ChessGuru** → **App Information** → **Privacy Policy URL**.

## Email confirmation redirect (Supabase)

After you push `email-verified.html`, add this URL in the Supabase dashboard:

1. **Authentication** → **URL Configuration**
2. **Redirect URLs** → add:
   `https://wc204-maker.github.io/ChessGuru-legal/email-verified.html`
3. Save

The app sends new sign-ups to that page when users tap the link in their inbox.
