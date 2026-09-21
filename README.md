# ohvar-site

**This repository is generated output. It is not the source of anything.**

It contains the built static site for [ohvar.com](https://ohvar.com) — exactly the
HTML, CSS and assets a browser already downloads when it visits the site. Nothing here is
private, because all of it is served publicly already.

## How it gets here

The source lives in a separate, private repository. On every push to that repository's
`main` branch, a GitHub Actions workflow runs `npm ci && npm run build` and pushes the
resulting `dist/` directory here, replacing the contents of this repository's default
branch. GitHub Pages then serves it.

Every commit here names the source commit it was built from, so the two can always be
correlated.

## Pull requests against this repository will be closed

Not out of rudeness — there is simply nowhere for a change here to go. Anything committed
to this repository is overwritten by the next build. Edits belong upstream in the source
repository, where they can be reviewed against the content rules the site is held to.

If you have found a problem with the site — a typo, a broken link, a wrong claim — please
open an issue here describing it, or email the address on the site's contact page. That
reaches the people who can fix it at the source.

## What lives where

| | source repository (private) | this repository (public) |
|---|---|---|
| Site source, components, copy | yes | no |
| Issues, review history, planning | yes | no |
| Built HTML/CSS/assets | build artifact, not committed | yes, and only this |
| Where to file a change | here | not here |

<!-- web#97 key-rotation mirror-proof: forcing a real diff so the push path (not just skip-if-unchanged) is exercised with the new key. Throwaway branch, never merged. -->
