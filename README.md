# frogchoir.lukemorse.dev

The site behind Frog Choir's share links, served by GitHub Pages.

- `.well-known/apple-app-site-association` lets iOS open
  `https://frogchoir.lukemorse.dev/p#<code>` in the app (team `4Z8CKPY35P`,
  bundle `com.lukemorse.frogChoir`). It must stay at that path with no extension,
  and must not redirect.
- `.nojekyll` stops Jekyll from dropping the `.well-known` folder.
- `p.html` is served at `/p` and is the page shown when the app isn't installed.
  The pond code is in the URL fragment, so it never reaches the server.
- `CNAME` holds the custom domain. DNS (Porkbun): `CNAME frogchoir → lukemorse.github.io`.

Pushing to `main` deploys.
