# my-app

A minimal static web app that displays **Hello World!** and **I'm Spiderman**.

## Project structure

```text
my-app/
├── index.html   # App markup and styles; no build step is required
└── README.md    # Setup and deployment notes
```

## Run locally

This is a plain static site. Open `index.html` in any modern browser to view it.

For a local server (useful if the project grows later), from the project folder run:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Change the displayed content

Open `index.html` and update the text in the `<h1>` and `<p>` elements near the
bottom of the file. The page's main colours are CSS custom properties under the
`:root` selector, so they can be changed in one place. Inline comments explain the
purpose of each section.

## Deploy with Cloudflare Pages

The app needs no framework preset, dependencies, or build command.

1. In the Cloudflare dashboard, go to **Workers & Pages** → **Create application** → **Pages** → **Connect to Git**.
2. Select the `my-app` repository.
3. Choose **None** (or no framework preset), leave **Build command** empty, and set **Build output directory** to `.`.
4. Click **Save and Deploy**.

Cloudflare Pages will redeploy automatically whenever you push changes to the
selected production branch.
