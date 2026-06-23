# Bus Website

A one-page static site with a centered Books logo, a daily zoomable map, and an inquiries email.

## Daily location update

Edit `map-location.js` and change this line:

```js
window.BOOK_BUS_LOCATION = "131 Avenue A, New York, NY 10009";
```

You can use an address, intersection, landmark, or exact coordinates:

```js
window.BOOK_BUS_LOCATION = "40.7268,-73.9818";
```

Commit the change to GitHub. Vercel will automatically redeploy the site.

The map defaults to satellite view via `window.BOOK_BUS_MAP_TYPE = "k";` in `map-location.js`.

## Deploy on Vercel

Use these settings:

- Framework Preset: Other
- Root Directory: ./
- Build Command: leave blank
- Output Directory: leave blank
- Install Command: leave blank

Make sure `index.html`, `styles.css`, `map-location.js`, and the `assets` folder are at the top level of the GitHub repo.


## Vercel Web Analytics

This site includes Vercel Web Analytics in `index.html` with:

```html
<script>
  window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>
```

Because this site is plain HTML/CSS/JavaScript rather than a Next.js app, you do **not** need to install `@vercel/analytics` or add a React component.

To start seeing data:

1. Make sure Web Analytics is enabled for this project in the Vercel dashboard.
2. Commit and push these files to GitHub.
3. Wait for Vercel to redeploy.
4. Visit the production site, then check the Web Analytics tab in Vercel.

If data does not appear after a minute or two, try disabling ad/content blockers and make sure you are checking the production deployment rather than a local file preview.
