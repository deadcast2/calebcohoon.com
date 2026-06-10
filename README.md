# calebcohoon.com

Personal portfolio site for Caleb Cohoon. Plain HTML/CSS/JS — no frameworks, no
build step, no dependencies. Everything (including images) is served from this
folder.

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Structure

```
index.html        the whole site (single page)
404.html          not-found page (used by GitHub Pages / Netlify automatically)
css/style.css     all styles; colors/fonts are CSS variables at the top
js/main.js        mobile nav + scroll-reveal, ~40 lines
assets/favicon.svg
assets/img/       project images (downloaded from GitHub READMEs, EXIF-stripped)
```

## Deploying to calebcohoon.com

Any static host works. Easiest options:

- **GitHub Pages**: push this folder to a repo, enable Pages (deploy from
  branch), then add `calebcohoon.com` as the custom domain (this creates a
  `CNAME` file). Point DNS: `A` records to GitHub Pages IPs + `CNAME` for
  `www`.
- **Netlify / Cloudflare Pages / Vercel**: drag-and-drop or connect the repo;
  no build command, publish directory = root. Add the custom domain in their
  dashboard and follow the DNS instructions.

Note: calebcohoon.com currently has **no DNS A record**, so you'll need to set
DNS at your registrar regardless of host.

## TODO — things only Caleb can fill in

Search `index.html` for `TODO(caleb)`:

1. **Unreal contest** — your 2010 blog post says you *won the grand prize
   ($500) at age 11* (for the original *Unreal*); your project notes said
   "runner up at 12". The site currently uses the blog's version. Confirm.
2. **Design Tech ×2** — both entries need the real "took them from X to Y"
   numbers.
3. **Bird of the Day, ThinkPDF/ThinkGFX, Remote Work, Xmas Quest, SAD,
   Log-a-Tour** — no public record survives; the current blurbs are minimal
   placeholders written from the names alone. Replace with real descriptions
   (and years if you remember them).
4. Consider swapping `assets/img/avatar.png` (your GitHub avatar, currently
   unused) for a real headshot if you want one in the hero.
5. **Links removed because they're dead** (as of 2026-06-09): your Mastodon
   profile (n64.social is unreachable), the Dispatch 27 SoundCloud (404), and
   github.com/calebhc/lunar_phase (404 — old account's repo is gone). If any
   come back or move, re-add them in the contact section.

## Recovered blog

The old blog (calebcohoon.blogspot.com, 2008–2016, "The Life of Caleb") is
preserved in the Wayback Machine. 25 of 34 posts were recovered with full text;
the missing 9 are from Jul/Aug/Dec 2008 and were never crawled. Key snapshots:

- Full-content Atom feed (25 posts, full HTML):
  https://web.archive.org/web/20160222140945/http://calebcohoon.blogspot.com/feeds/posts/default
- Homepage 2013: https://web.archive.org/web/20130506180230/http://calebcohoon.blogspot.com/
- Homepage 2016: https://web.archive.org/web/20160209021919/http://calebcohoon.blogspot.com/
