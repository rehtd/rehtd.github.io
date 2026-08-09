# Qunji Lin — Portfolio Site

A lightweight, responsive, single-page portfolio site for **Qunji Lin**, an aspiring AI Product Manager based in Hong Kong. Hosted on **GitHub Pages**.

- **Owner:** [github.com/rehtd](https://github.com/rehtd)
- **Live URL (after enabling Pages):** `https://rehtd.github.io/`
- **Stack:** Pure HTML, CSS, and vanilla JavaScript — no build step, no external dependencies.

---

## Project Structure

```
.
├── index.html      # Single-page site (Hero, About, Projects, Skills, Certifications, Contact)
├── styles.css      # All styling, responsive layout, dark-navy hero theme
├── script.js       # Sticky header, mobile nav toggle, reveal-on-scroll animations
└── README.md       # You are here
```

The site is a **single page with anchor navigation**. There is no bundler, no framework, and no third-party CDN — it loads instantly and works offline once cached.

---

## Local Preview

You can open `index.html` directly in a browser, but for a slightly more realistic preview (especially for scroll behavior and mobile testing), use a simple local HTTP server.

### Option A — Python 3 (recommended, no install)

```bash
# from the project root
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

### Option B — Node.js

```bash
npx serve .
# or
npx http-server -p 8000
```

### Option C — VS Code

Install the **Live Server** extension, right-click `index.html` → **Open with Live Server**.

---

## Deploy to GitHub Pages

This repo is named `rehtd.github.io`, which means it will be served from the user root (`https://rehtd.github.io/`) — no `/portfolio` subpath to worry about.

### One-time setup (do this in the GitHub web UI)

1. Go to `https://github.com/rehtd/rehtd.github.io/settings/pages`.
2. Under **Source**, select **Deploy from a branch**.
3. Choose:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**.
5. Wait ~1 minute. GitHub will show the live URL at the top of the same page.

> If the **Pages** menu is missing or disabled, GitHub may require you to first push at least one commit to `main` (already done in this repo) and to verify your email address.

### How updates work

Just `git push` to `main`. GitHub Actions / the Pages bot will rebuild and publish within ~30 seconds. No CI configuration is required for a pure-static site.

---

## Customization Checklist

Once Pages is live, the most common edits are:

- [ ] **Replace the two project cards** in `index.html` (`#projects`) with real case studies — add images, GitHub links, write-ups.
- [ ] **Update `About`** paragraph with your final wording.
- [ ] **Add LinkedIn** URL in the **Contact** section.
- [ ] **Add an avatar / headshot** — drop a file like `avatar.jpg` next to `index.html` and add a small image in the hero.
- [ ] **Add a `CNAME`** file (optional) if you want to use a custom domain.

---

## License

MIT — feel free to fork and adapt for your own portfolio.
