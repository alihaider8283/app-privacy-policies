# App Privacy Policies

Privacy policies for my mobile apps, hosted free on GitHub Pages.

| App | Policy URL |
|-----|-----------|
| My App | `https://<username>.github.io/app-privacy-policies/my-app/` |

## Add a new app

1. Copy `_template/` to a new folder with a short URL-friendly name, e.g. `cp -r _template fit-track`.
2. Edit `fit-track/index.html`: replace every `[PLACEHOLDER]` and delete the data sections that don't apply.
3. Add a link to it in the root `index.html` (and the table above).
4. Commit and push. The policy will be live at `https://<username>.github.io/app-privacy-policies/fit-track/`.

## First-time deploy

```bash
git init
git add .
git commit -m "Add privacy policies"
# create an empty PUBLIC repo named app-privacy-policies on github.com, then:
git remote add origin https://github.com/<username>/app-privacy-policies.git
git branch -M main
git push -u origin main
```

Then on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `(root)` → Save**.
After a minute or two the site is live at `https://<username>.github.io/app-privacy-policies/`.

## Preview locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```
