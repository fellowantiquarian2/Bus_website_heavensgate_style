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
