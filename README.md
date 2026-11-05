# Shiftalya legal site (GitHub Pages)

Static support and privacy pages for the **Shiftalya** mobile app (version 1.0.0). No build step or dependencies.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Support / home page |
| `privacy.html` | Privacy policy (English, Deutsch, Türkçe) |
| `styles.css` | Shared responsive styles |

## Publish to `shiftalya-legal` on GitHub Pages

These files are meant to live in the public repository **`shiftalya-legal`**, served from the **root of the `main` branch**.

### Option A — This folder is the only content of `shiftalya-legal`

1. Create the repo on GitHub: `shiftalya-legal` (public).
2. Upload these files to the **repository root** on `main` (from this machine: `C:\Users\bartu\Desktop\Shiftly\shiftalya-legal-site\`):
   - **Required for Pages:** `index.html`, `privacy.html`, `styles.css`
   - **Optional:** `README.md` (maintainer docs; not required for the live site)
   - Do **not** upload the Shiftalya app, `node_modules`, or other parent folders.
3. Commit and push to `main`.
4. On GitHub: **Settings → Pages**
   - **Source:** Deploy from a branch
   - **Branch:** `main` / **Folder:** `/ (root)`
   - Save
5. After a minute or two, the site is available at:
   - `https://<your-github-username>.github.io/shiftalya-legal/`
   - Privacy URL for stores: `https://<your-github-username>.github.io/shiftalya-legal/privacy.html`

### Option B — Push from this monorepo path (subfolder)

GitHub Pages cannot serve a subfolder of another repo by default. Either use a **separate** `shiftalya-legal` repo (recommended above), or use a GitHub Action in `shiftalya-legal` that copies artifacts from elsewhere. For the simplest store setup, use **Option A**.

### Custom domain (optional)

In **Pages → Custom domain**, add your domain and configure DNS per GitHub’s instructions.

## Local preview

Open `index.html` in a browser, or use any static server:

```powershell
cd shiftalya-legal-site
npx --yes serve .
```

## Contact

Privacy and support email referenced on the site: **contact.bar2run@gmail.com**
