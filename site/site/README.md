# Chef Kym's — website

Static single-page site for Chef Kym's (1188 N Range St, Dothan, AL).
Pages (Home, Menu, Book, Shop, About) are sections of one page with a horizontal slide transition.

## Structure

```
site/
  index.html      the whole site (markup + logic)
  support.js      runtime that renders index.html
  uploads/        photography and the brand seal
```

## Run locally

Any static server, e.g.:

```bash
cd site
python3 -m http.server 8000
```

Then open http://localhost:8000

## Deploy

No build step — point any static host at `site/`.

- **Vercel:** import the repo, framework preset "Other", output directory `site`.
- **Netlify:** publish directory `site`, build command empty.
- **GitHub Pages:** push, then Settings → Pages → deploy from branch, folder `/site` (rename to `/docs` if Pages requires it).

## Booking

"Book now" on the Book page links to her Setmore calendar: https://chef6axk.setmore.com

## Before launch

- Re-upload the product and catering photos that came from the old Wix site so nothing depends on it.
- Confirm merch prices (apron, tee, cup, pop socket) and the 32 oz seasoning photo.
- Add her booking phone number (the site currently shows the restaurant line, 334-699-5005, only for the restaurant).
