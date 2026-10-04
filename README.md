# JWT Viewer

JWT Viewer decodes a JSON Web Token in the browser and shows the header and payload as formatted JSON. The token never leaves the page.

**Live app:** https://jwt.sanjaysingh.net

## What it does

Paste or type a token in the input. The page splits the token on `.`, base64-decodes the header and payload, and pretty-prints both. A sample token is filled in so the layout is visible immediately. Malformed input shows an error instead of partial output.

The signature segment is not verified. This page does not check the signing key, expiry, or issuer. Use it to inspect claims, not to decide whether a token is authentic.

## Privacy

Decoding runs entirely in the browser. There is no server, account, or stored history.

## Run locally

Open `index.html` in a browser. Bootstrap and Prism load from a CDN, so those assets need a network connection. No install or build step is required.

## Deploy

Commits that land on `main` deploy to GitHub Pages at https://jwt.sanjaysingh.net. Changes reach `main` through a pull request.
