# Your personal website

A fast, dependency-free static site (plain HTML/CSS/JS). No build step, no
frameworks — it works the moment you open `index.html`, and it's ready to
publish free on GitHub Pages under your own account.

## Files

| File          | What it's for                                          |
| ------------- | ------------------------------------------------------ |
| `index.html`  | All the content. Search for `EDIT ME` comments.        |
| `styles.css`  | All the styling. Colors live in `:root` at the top.    |
| `script.js`   | Footer year + gentle scroll reveals.                   |
| `.nojekyll`   | Tells GitHub Pages to serve the files as-is. Leave it. |

## 1. Make it yours (5 minutes)

Open `index.html` in any text editor and look for the `EDIT ME` comments:

- Your name, role, and intro (the hero section)
- Your projects (duplicate a `<li class="work-item">` block to add more)
- Your about text and the facts panel
- Your real email and social links (in the contact section)

Change the page title and `<meta name="description">` at the top too — that's
what shows in browser tabs and search results.

**Want a different accent color?** Open `styles.css` and edit `--accent` and
`--accent-soft` near the top. Everything updates automatically.

## 2. Publish it on GitHub Pages

You own your GitHub account, so publishing here means the site is yours from
the very first second — nothing to hand over later. Pick whichever route feels
comfortable.

### Route A — no terminal, all in the browser (easiest)

1. Go to <https://github.com/new> and create a repository.
   - Name it `your-username.github.io` (use your actual GitHub username) to get
     the clean URL `https://your-username.github.io`.
   - Or name it anything, e.g. `website` — the URL will then be
     `https://your-username.github.io/website`.
   - Set it to **Public**.
2. On the new repo page, click **uploading an existing file**.
3. Drag in every file from this folder — including the hidden `.nojekyll`.
   (On Mac press `Cmd+Shift+.` in Finder to see hidden files; on Windows enable
   "Hidden items" in the View tab.)
4. Click **Commit changes**.
5. Go to **Settings → Pages**. Under **Build and deployment → Source**, choose
   **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder,
   then **Save**.
6. Wait ~1 minute, refresh, and your live URL will appear at the top of that
   Pages screen.

### Route B — command line (if you use git)

```bash
# from inside this folder
git init
git add .
git commit -m "Initial site"
git branch -M main

# create an EMPTY repo on github.com first, then:
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin main
```

Then do step 5 above (**Settings → Pages**) to turn Pages on.

## 3. Updating later

Edit the files and re-upload them (Route A), or `git add . && git commit -m
"update" && git push` (Route B). GitHub Pages redeploys automatically within a
minute or so.

## Notes

- Custom domain? In **Settings → Pages → Custom domain**, add your domain and
  follow GitHub's DNS instructions.
- The fonts load from Google Fonts over the internet; no setup needed.
- Everything here is yours to change however you like.
