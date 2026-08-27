# Re-Seat Website — GitHub Hosting Guide

This folder contains a simple static website for the Re-Seat app.
Host it free with **GitHub Pages**.

## 1. Create a GitHub repository
Sign in at https://github.com and create a new repository, e.g. `re-seat` (public).

## 2. Push this folder
```bash
cd website
git init
git add .
git commit -m "Re-Seat website"
git branch -M main
git remote add origin https://github.com/<your-username>/re-seat.git
git push -u origin main
```

(You can also drag the files into a new repo via the GitHub web interface.)

## 3. Enable GitHub Pages
- Repo → **Settings → Pages**
- Source: **Deploy from a branch** → branch `main`, folder `/ (root)` → Save

Your site will be live at:
`https://<your-username>.github.io/re-seat/`

## 4. (Optional) Custom domain
- Buy a domain (e.g. re-seat.app), add it in Pages settings, and add a `CNAME` file containing the domain.

## 5. Update the App Store link
In `index.html`, replace the placeholder link:
```html
<a class="appstore" href="#">Download on the App Store</a>
```
with your real link (visible in App Store Connect once the app is approved),
e.g. `https://apps.apple.com/app/idXXXXXXXXXX`.

## 6. Point App Store Connect here
Use these URLs when submitting:
- Privacy policy: `https://<your-username>.github.io/re-seat/privacy.html`
- Support: `https://<your-username>.github.io/re-seat/support.html`
