# Public App Pages

Static HTML pages designed to publish directly from `https://mikeisman.github.io/`.

Each application gets its own top-level folder so public URLs stay clean and predictable:

- `https://mikeisman.github.io/weightroom/support.html`
- `https://mikeisman.github.io/parenthub/privacy.html`

## Pages

- `index.html` - Directory page for all public app pages
- `weightroom/index.html` - Weightroom app page index
- `weightroom/support.html` - Weightroom support page
- `parenthub/index.html` - ParentHub app page index
- `parenthub/privacy.html` - ParentHub privacy page

## Add Another App

1. Create a new top-level folder, for example `newapp/`.
2. Add static pages inside it, such as `support.html`, `privacy.html`, or `terms.html`.
3. Link to shared assets with `/assets/site.css` and `/assets/site.js`.
4. Add the new app to the root `index.html` directory.

## Local Preview

Open `index.html` in a browser, or run a tiny local server:

```sh
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Publish On GitHub Pages

1. Push this repository to GitHub as `mikeisman.github.io`.
2. In the GitHub repository, go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder.
5. Save. GitHub will publish the site at `https://mikeisman.github.io/`.
