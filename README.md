# Kana Kaanum Kalangal

A small, quiet keepsake website for Karthiyayini and Naveen. It is a single static page (`index.html`) with no build step, no backend and no dependencies.

## What it includes

- **Home:** live day counter from 12 December 2025, today's reason, next special date, a random love note
- **Our Story:** editable timeline (only 12 December 2025 is pre-dated; fill in the rest yourselves)
- **Our World:** 365 numbered, editable reasons, and the soundtrack (6 songs with Spotify links, favourites and notes, no autoplay)
- **More:** letters (love letters, birthday wishes, anniversary messages, open-when, personal notes, future letters, promises, love notes) with search, a bucket list, and special dates with countdowns

## Files

```
index.html   the whole site (HTML, CSS and JavaScript)
README.md    this file
.gitignore
```

## Run it on your computer

Open `index.html` in any browser. That's all.

## Publish it with GitHub Pages

1. Create a GitHub account and click **New repository**. Name it, for example, `kana-kaanum-kalangal`.
2. Upload `index.html`, `README.md` and `.gitignore`. On a phone or in a browser: **Add file → Upload files**, then **Commit changes**.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then **Save**.
5. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/kana-kaanum-kalangal/`.

Or from a terminal:

```
git init
git add .
git commit -m "first version"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/kana-kaanum-kalangal.git
git push -u origin main
```

## Privacy: please read

- GitHub Pages on a free account needs a **public** repository. Private-repo Pages requires a paid GitHub plan.
- There is **no login**. Anyone who has the site address can open it, and anyone can read the code, including the starter text in the first eight reasons.
- Pick a repository name that is not easy to guess, and share the link only with each other.
- Nothing you type is sent anywhere. Everything you write (reasons, letters, notes, goals, dates) is saved in **your own browser only**, so it never appears in the repository or on GitHub.
- If you want real privacy with a login, you need a backend. That is the larger Node, PostgreSQL and Better Auth version, which has to be built separately.

## Data and backups

- Each person sees only what was typed on their own browser and device. You and Naveen will not see each other's entries.
- Clearing browser data, or using a private window, erases what was saved.
- There is no export button in this version. Keep important letters copied somewhere safe too.

## Customising

All of it is in `index.html`:

- **Start date:** search for `var START=new Date(2025,11,12)` (the month is zero-based, so 11 means December).
- **Starter reasons, story entries, songs, dates:** edit the `SEED` object near the top of the script.
- **Colours and fonts:** edit the `:root` variables and the `font-family` lines at the top of the file.
- **Songs:** each Spotify link is a search link, so it opens Spotify and finds the song in the listener's own account.

Changes to seed text only affect people who have not saved their own data yet. Anything already saved in a browser stays as it was.

## Limitations

- No login, no shared database, no password reset.
- No quizzes, no export, no photo or video features.
- Fonts load from Google Fonts. If they are blocked, the page falls back to Georgia.
