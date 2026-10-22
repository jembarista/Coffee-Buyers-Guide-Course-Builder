# Coffee Buyers Guide Course Builder

A Barista Hustle × Sucafina workspace for developing The Coffee Buyer's Guide to Burundi, focused on Arabica.

## Run

Serve this folder with any static HTTP server, then open index.html. No dependencies or build step are required. For example:

```sh
python3 -m http.server 8000
```

Visit http://localhost:8000. Use a consistent origin and port to retain access to the same browser storage.

## Current features

- 42 lessons following the Guatemala course structure.
- Lesson research questions, answers, evidence links, editable interview questions and lesson drafts.
- Chapter and status filters, search and progress tracking.
- Eight proposed filming sessions grouping footage across lessons. No chapter introduction or recap videos.
- Terroir Map links for origin and climate activities.
- JSON answer pack export and import.
- HTML course draft and interview brief exports.

## Data and backups

Answers are saved in browser localStorage under `bh-burundi-v1`. There is no server database, account system, shared editing or automatic external backup. Browser data does not travel with the source code and can be lost if browser storage is cleared. Export answer packs regularly and retain them in a backed-up shared location. Import replaces matching lesson records after confirmation; it does not resolve concurrent edits.

Keep question order stable: answers currently use question array positions. Stable question IDs are a prerequisite for reliable document round trips.

## Files

- `index.html` — app shell
- `style.css` — responsive interface
- `data.js` — course lessons, research and interview questions, filming sessions
- `app.js` — editing, browser storage and exports
- `docs/` — Word drafting template, predating the app's reduced filming plan
- `docs/ROADMAP.md` — agreed direction and outstanding work

No live Google Docs integration, photo uploads or media library connection is implemented. The app has not been deployed from this repository.
