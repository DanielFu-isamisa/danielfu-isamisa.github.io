# Daniel Fu: personal site

A single-page static site: `index.html` plus the `img/` folder. No build step.

## Make it a public, shareable link (GitHub Pages, free, about 10 minutes)

**1. Make a GitHub account.** Go to github.com and sign up (free). Your username
becomes part of the link, so pick one that looks fine to an admissions reader,
for example `danielfu` or `danielfu27`.

**2. Create the repository.** Click **+** (top right) → **New repository**.
- Repository name: exactly `YOUR-USERNAME.github.io` (all lowercase, e.g. `danielfu.github.io`).
- Visibility: **Public**. On a free account, Pages only works for public repositories.
- Leave everything else as is and click **Create repository**.

**3. Upload the site.** Unzip `danielfu-site.zip` on your computer first.
On the new repo's page, click **uploading an existing file** (or **Add file → Upload files**).
Open the unzipped `danielfu-site` folder and drag in what's **inside** it:
`index.html`, `README.md` and the `img` folder. Use Chrome or Edge so the `img`
folder keeps its name. `index.html` must sit at the top level of the repo, not inside
another folder. Wait for all files to finish uploading, then click **Commit changes**.

**4. Turn on Pages.** In the repo, go to **Settings → Pages** (left sidebar).
Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to
**main** and folder to **/ (root)**, then click **Save**.

**5. Get the link.** After a minute or two, refresh the Pages settings page. It shows
"Your site is live at `https://YOUR-USERNAME.github.io`". Click **Visit site**.

**6. Check it the way others will see it.** Open the link in a private/incognito
window and on your phone. If it loads there, anyone you send it to can see it.
No login is needed to view it.

### If something goes wrong
- **404 page:** wait 2–3 minutes and refresh. Then check that `index.html` is at the
  top level of the repo (you should see it listed on the repo's main page, not inside
  a `danielfu-site` folder).
- **Pictures missing:** the `img` folder didn't upload. Use **Add file → Upload files**
  again and drag in the `img` folder.
- **Repo is private:** Settings → General → scroll to **Danger Zone** →
  **Change visibility** → **Make public**.
- **Want a different link name:** a repo named anything else (say `portfolio`) works
  too, but the link becomes `https://YOUR-USERNAME.github.io/portfolio/`.

## Changing something later

Open `index.html` on GitHub, click the pencil icon, edit and **Commit changes**.
The live site updates within a minute or two.

## Adding finished photos for the "process only" art pieces

Tree, foot, eye (3D) and bird (drawing) currently show process boards only.
To add a finished photo:

1. Save a JPEG about 2000 px on the long side as `img/tree-1.jpg`, plus a
   copy about 760 px on the long side as `img/tree-1-t.jpg`.
2. In `index.html`, find the line `{id:'tree',t:'tree',final:[],proc:['tree-p']}`
   and change it to
   `{id:'tree',t:'tree',final:['tree-1'],proc:['tree-p'],cap:['One-line description.']}`.
3. Upload both files and the edited `index.html`.
