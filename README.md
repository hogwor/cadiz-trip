# Cádiz Meet Week

A single-page trip guide for the Kaiserslautern Kingfish trip to Cádiz, Spain —
**23–30 November 2026**. Built around the meet weekend (Fri evening, Sat, Sun).

Six tabs: **Trip · Days · Meet · Drive · Stay · To Do**. Mobile-first, works offline
once loaded, checklist state saves per-device in the browser.

## Share it on GitHub

Everything is in `index.html` — no build step, no dependencies. Only external
request is Google Fonts (Oswald + Source Sans 3), which falls back cleanly.

```bash
git init && git add . && git commit -m "Cádiz trip guide"
```

Then create the repo and enable Pages:

```bash
gh repo create cadiz-trip --public --source=. --push
```

In the repo: **Settings → Pages → Source: Deploy from a branch → `main` / `root`**.
Live in a minute or two at `https://<your-username>.github.io/cadiz-trip/`.

Anyone with the link can open it — no account needed. Fine for sharing with other
swim families.

## Editing

Content is plain HTML inside the six `<section class="panel">` blocks. Colors are
CSS custom properties at the top of the `<style>` block — team royal `#0030A8`,
red `#D81830`, taken from the Kingfish crest.

## Notes

- Countdown and day math are computed from the 23 Nov 2026 departure.
- Hotel details were gathered from public listings and should be confirmed at booking.
- Meet session times are not yet confirmed — they drive the Sunday departure plan.
