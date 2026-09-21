# notes

A single static page that displays notes shared with a **Web Annotator** view link.

Two kinds of link:

- `…/#v1.<data>` — the notes are carried entirely inside the URL fragment. Browsers never send
  fragments to a server, so this page decodes them locally.
- `…/?g=<gist id>` — a live link: the page reads a secret GitHub gist kept up to date by the
  sharer's extension (their notes plus a cleaned copy of the document) and re-checks it for changes.

Either way this site stores nothing and contains no one's notes. Shared documents are rebuilt
through a strict tag allowlist; no fetched or decoded text is ever inserted as HTML.

`index.html` is self-contained — no dependencies, no network requests.
