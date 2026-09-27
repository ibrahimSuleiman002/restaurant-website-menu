# Ember & Olive

A responsive static restaurant website with home, menu, story, gallery, reservations, contact, authentication, password recovery, and account-management views.

## Run locally

No build step or backend is required. Serve the folder with any static web server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

Opening `index.html` directly also works in most browsers, but a local server gives the most accurate preview.

## Deploy with GitHub Pages

1. Create a new GitHub repository.
2. Upload every file and folder from this package, including `.github` and `.nojekyll`.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **GitHub Actions**.
5. Push to the `main` branch. The included workflow publishes the site automatically.

The deployed URL will appear in the workflow run and in **Settings → Pages**.

## Data and authentication

Accounts, passwords, recovery codes, reservations, messages, and history are stored only in the visitor's browser using `localStorage` and `sessionStorage`. There is no server or database. Data does not sync between devices or browsers.

## Project files

- `index.html` — document shell, navigation, footer, confirmation dialog
- `style.css` — responsive layout and styling
- `app.js` — page rendering, forms, local authentication, reservations, and account controls
- `.nojekyll` — prevents GitHub Pages from applying Jekyll processing
- `.github/workflows/pages.yml` — automatic GitHub Pages deployment

## Photography

Photography is loaded from Unsplash and remains subject to the [Unsplash License](https://unsplash.com/license):

- [Pasta being lifted with a fork](https://unsplash.com/photos/qfpVo7fMyII)
- [Pasta on a plate](https://unsplash.com/photos/jL3X9oeQ3Ps)
- [Burrata with tomatoes and herbs](https://unsplash.com/photos/x-EakqrXIuk)
- [Tiramisu in Italy](https://unsplash.com/photos/4hyLfxa06dQ)
- [Rustic restaurant interior](https://unsplash.com/photos/Q73XXHcIsa8)

## Notes

The site is fully static. External network access is required for the Unsplash photographs to load.
