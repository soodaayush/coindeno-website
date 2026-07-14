# CoinDeno Website

![coindeno-website](https://github.com/user-attachments/assets/ec3eeca5-5062-44f7-a2f3-a26cab4a4afc)

The official marketing website for [CoinDeno](https://github.com/soodaayush/coindeno), a mobile app for tracking cryptocurrencies.

**Live site:** https://coindeno.netlify.app/

## What's here

A static, no-build-tool site with two pages:

- `index.html` &mdash; the landing page
- `privacyPolicy.html` &mdash; the app's privacy policy

## Project structure

```
.
├── index.html
├── privacyPolicy.html
├── scss/styles.scss   # source styles
├── css/styles.css     # compiled, compressed CSS served by the site
├── images/
├── fonts/
├── site.webmanifest
└── robots.txt
```

## Developing locally

Serve the directory with any static file server, e.g.:

```sh
python3 -m http.server 8080
```

Then open http://localhost:8080.

Styles are authored in `scss/styles.scss` and compiled to `css/styles.css`. After editing the SCSS, recompile with [Sass](https://sass-lang.com/):

```sh
npx sass scss/styles.scss css/styles.css --style=compressed --no-source-map
```

Commit both the `.scss` source and the compiled `.css` output.

## Deployment

The site is deployed on [Netlify](https://www.netlify.com/) and redeploys automatically from the `main` branch.
