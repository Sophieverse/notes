# notes

A single static page that displays notes shared with a **Web Annotator** view link.

The notes are carried entirely inside the link's URL fragment (`#v1.…`). Browsers never send
fragments to a server, so this page decodes them locally: nothing is uploaded, stored, or
logged, and the site itself contains no one's notes.

`index.html` is self-contained — no dependencies, no network requests.
