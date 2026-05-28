# sona pona — toki pona trainer

A tiny, gentle trainer for [toki pona](https://tokipona.org), the ~130-word
"language of good." Lessons, a dictionary, a grammar guide, and spaced-repetition
flashcards — all in a single HTML file.

Progress is saved on your device and, when you sign in, synced to the cloud via
Firebase so you can pick up on any device.

## Files

- `index.html` — the entire app (HTML, CSS, and JavaScript in one file).
- `README.md` — this file.

## Running it

Just open `index.html` in a browser, or host it anywhere that serves static
files. It's deployed on GitHub Pages.

## Cloud sync (Firebase)

The app works fully offline with no setup. Cloud sync is optional and turns on
once you paste your own Firebase config into `index.html` (look for
`FIREBASE_CONFIG` near the top of the `<script>`).

Firebase **web API keys are public by design** — they're meant to ship in
client-side code. Security comes from the Realtime Database *rules*, not from
hiding the key, so it's safe to commit the config to a public repo.

A note on the optional password: it's a light convenience guard so a stranger
can't load your data just by typing your username. It is **not** real
authentication (it's stored in the database as-is), so don't reuse an important
password here.

## Credits

Language content is built from the official *pu* word list
(Sonja Lang, *Toki Pona: The Language of Good*).
