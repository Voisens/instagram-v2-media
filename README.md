# instagram-v2-media

Public media host for the [instagram-v2](https://github.com/Voisens/instagram-v2) pipeline.

This repo holds **rendered slide images only** — no pipeline source code, prompts,
or secrets. It exists because the Instagram Graph API's Content Publishing
endpoint fetches media from a public URL rather than accepting a direct file
upload; this repo + GitHub Pages is that public URL.

Files are pushed here by `graph_api/client.py`'s `host_file()` immediately
before each publish call, and are expected to become public shortly before
they're posted to Instagram anyway — no image is ever hosted here that
isn't already headed for the public feed.

Served via GitHub Pages at `https://voisens.github.io/instagram-v2-media/`.
