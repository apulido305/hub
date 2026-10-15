# mrpulido.com

Central app hub for Mr. Pulido's study games. Live at https://mrpulido.com.

A single static page (`index.html`, no build step) served by GitHub Pages from `main`.

This is a project repo (`apulido305/hub`), not the GitHub user site, so the custom domain applies only to the hub.
The games are served from `https://apulido305.github.io/<repo>/`, because the school wifi blocks mrpulido.com.

## Apps linked

| App | Live URL | Repo |
|---|---|---|
| Elemental Arcade | https://apulido305.github.io/elemental-arcade/ | [elemental-arcade](https://github.com/apulido305/elemental-arcade) |
| Cell Arcade | https://apulido305.github.io/cell-arcade/ | [cell-arcade](https://github.com/apulido305/cell-arcade) |
| Space Arcade | https://apulido305.github.io/earthspace/ | [earthspace](https://github.com/apulido305/earthspace) |
| Code Arcade | https://apulido305.github.io/code-arcade/ | [code-arcade](https://github.com/apulido305/code-arcade) |
| Scripture Arcade | https://apulido305.github.io/bible-arcade/ | [bible-arcade](https://github.com/apulido305/bible-arcade) |
| Math Arcade | https://apulido305.github.io/math-arcade/ | [math-arcade](https://github.com/apulido305/math-arcade) |
| Spelling Flashcards | https://apulido305.github.io/spelling/ | [spelling](https://github.com/apulido305/spelling) |
| Multiplication Practice | https://apulido305.github.io/multiplication/ | [multiplication](https://github.com/apulido305/multiplication) |

## Adding an app

1. Turn on GitHub Pages in the app's repo; it appears at `apulido305.github.io/<repo-name>/`.
2. Copy an `<article class="tile">` block in `index.html` and change the link (`https://apulido305.github.io/<repo-name>/`), text, `data-cat` and `data-keys`.
3. Add it to the `APPS` object in the script so the Quick CLI can launch it.
4. If it is a new subject, add a pill and sidebar button with a matching `data-filter`.

## Domain (Cloudflare DNS)

`CNAME` holds `mrpulido.com`. In Cloudflare DNS, set these records to **DNS only** (grey cloud) until GitHub issues the HTTPS certificate:

- `A` `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `CNAME` `www` → `apulido305.github.io`

`design/` holds the original mockup (`code.html`, `screen.png`) and is not linked from the site.

