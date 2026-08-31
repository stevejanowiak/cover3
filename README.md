# Cover Three

Everything lives in `index.html`. No build step, no server, no dependencies
to install once it's live — just a page.

---

## First-time setup (about 10 minutes)

1. **Create a GitHub account** at github.com if you don't have one.

2. **Create a repository.** Click the `+` in the top right, then *New repository*.
   - Name it something like `cover-three`
   - Set it to **Public** — GitHub Pages is only free on public repos
   - Check *Add a README file*
   - Click *Create repository*

3. **Upload the dashboard.** In the repo, click *Add file* → *Upload files*,
   drag in `index.html`, then click *Commit changes*.
   The filename must be exactly `index.html` — that's what Pages serves by default.

4. **Turn on Pages.** Go to *Settings* → *Pages* (left sidebar).
   Under *Source*, choose **Deploy from a branch**. Set branch to `main` and
   folder to `/ (root)`. Click *Save*.

5. **Wait about a minute**, then reload the Settings → Pages screen. Your URL appears at
   the top, in the form:

   ```
   https://YOURNAME.github.io/cover-three/
   ```

   Send that link to Matt and Dan. No account or login needed on their end.

---

## Weekly update

After Claude Code processes a week's picks and rebuilds `index.html` (see
`WORKFLOW.md` in your local project folder), publish it:

1. Open your repo and click on `index.html`
2. Click the pencil icon (*Edit this file*), select all, and paste in the new contents
   — or use *Add file* → *Upload files* and drop the new one in to overwrite
3. Click *Commit changes*
4. The live site updates in under a minute

Every commit is saved, so the *History* tab lets you see or roll back any
prior week's version.

---

## What belongs in this repo (and what doesn't)

Only `index.html` and this README should ever go here. The scripts that
generate it — `cli.js`, `lib.js`, `build.js` — and the season data behind
it, including **Matt's and Dan's email addresses and every pick they've
made**, stay on your own computer in the `cover-three-code` folder Claude
Code works from.

Don't upload `season.json` or `config.json` to this repo. This has to be a
public repo for free GitHub Pages hosting, which means anything in it is
visible to anyone — that's fine for the dashboard itself, not for their
inboxes.

---

## Notes

- Public means public. No login wall on this page — anyone with the link
  can see standings, picks, and results. Presumably fine among the three of
  you, but worth remembering before the link goes anywhere else.
- Naming the repo `YOURNAME.github.io` instead serves it at your root URL
  with no subfolder — only works for one repo per account. A named repo
  like `cover-three` is the safer default if you might host something else
  there later.
