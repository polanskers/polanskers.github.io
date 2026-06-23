# Mia Polansky personal site

Static GitHub Pages site for `github.com/polanskers/polanskers.github.io`.

## Publish

1. Create a new public GitHub repo named `polanskers.github.io` under the `polanskers` account.
2. From this folder, run:

   ```sh
   git init
   git add .
   git commit -m "Create personal site"
   git branch -M main
   git remote add origin git@github.com:polanskers/polanskers.github.io.git
   git push -u origin main
   ```

3. In GitHub, open Settings -> Pages and make sure the source is `main` / root.
4. The default URL will be `https://polanskers.github.io/`.

## Custom domain

An email address is not a URL. When you know the actual domain, add a file named `CNAME` containing only the domain, for example:

```txt
miapolansky.com
```

Then configure DNS wherever you bought the domain:

- `A` records for the root domain pointing to GitHub Pages.
- `CNAME` record for `www` pointing to `polanskers.github.io`.

GitHub's Pages settings will show the exact DNS status after you enter the domain.

## Edit content

- Main copy and links: `index.html`
- Visual styling: `styles.css`
- Tiny navigation behavior: `script.js`
- CV asset: `assets/Mia_Polansky_CV.pdf`
