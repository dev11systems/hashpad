# #hashpad

Plain text notes that live in the URL.

#hashpad is a minimalist, client‑side notepad where the entire document is stored in the `#hash` portion of the URL. There is no server, no account, and no backend.

Copy the URL and you’ve copied the note.

---

## What it is

* A single‑page, zero‑dependency web app
* Plain‑text only (no rich text, no formatting surprises)
* Notes are compressed and embedded directly in the URL
* Designed to work offline and on mobile

## What it is *not*

* Not a collaborative editor
* Not a cloud sync service
* Not designed for binary data or large media

---

## How it works

1. You type into a plain‑text editor
2. The text is compressed in your browser
3. The compressed data is stored in the URL fragment (`#`)
4. Sharing the link shares the note

If a note becomes too large or too high‑entropy to fit safely in a URL, #hashpad automatically falls back to **local‑only storage** in your browser.

---

## Features

* URL‑based notes (shareable, bookmarkable)
* Automatic save as you type
* Local‑only fallback for large notes
* Optional AES‑GCM encryption for sharing
* Export to `.txt` or `.md`
* Session resume prompt
* Tab titles derived from note content
* Keyboard‑friendly
* Mobile‑friendly

---

## Privacy model

* Shareable links are readable by anyone with the URL
* Encrypted links store only ciphertext in the URL
* Passphrases are never stored or transmitted
* Local‑only notes never leave your browser

---

## Usage

* Open the base URL to start a new note
* Paste or type plain text
* Copy the URL to share
* Use browser history to recover past notes

Keyboard shortcuts are documented in the in‑app About panel.

---

## Directory structure (suggested)

```
/
├─ index.html        # main app
├─ about/
│  └─ index.html    # static about page
├─ README.md
├─ LICENSE
```

---

## Philosophy

#hashpad is intentionally small.

It avoids accounts, servers, sync, and abstraction layers. The goal is a tool that feels closer to a scratchpad than a platform.

---

## License

MIT (recommended)

---

#hashpad — plain text • no server • no account
