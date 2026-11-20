# Bolsonaro Hospital Tracker

A static site (GitHub Pages) with a calendar and charts of every day Jair Bolsonaro has spent in a hospital since the 6 September 2018 stabbing, compiled from news reports.

## Updating

All data lives in [`data.js`](data.js).

- **New admission:** add an entry with `end: null`. The site counts an open stay up to today (Brasília time), so it stays current without further edits.
- **Discharge:** set `end` to the discharge date (`"YYYY-MM-DD"`).
- Add the reports you used to `SRC` and list their keys in the entry's `sources`.

No build step: `index.html` + `data.js` are served as-is.
