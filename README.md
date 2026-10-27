# The Spot Fake Media Guide

Believe less, verify more — explained like a friend would. A beginner's
manual for checking the media you meet in a normal scrolling day:

- spotting **AI-made images** with the zoom-in habit (hands, text,
  reflections, shadows, background melt),
- reading **fake screenshots** for their seams — "receipts" that aren't,
- listening past **cloned voices** and "leaked audio",
- watching **deepfake video** with an editor's eyes (and the slow-motion
  trick),
- the single best tool anyone can learn: **reverse image search**,
- **provenance labels (C2PA)** — the receipts more and more content
  carries, and how to read them,
- **asking AI to check AI** — three prompt recipes and the honest limits,
- **family group chat habits** and kind scripts that slow the spread,
- a calm, five-minute **believe-less-verify-more playbook** with a
  legitimate "unresolved" verdict,
- five **practice scenes** with expandable answers, a printable
  **checklist**, and a plain-English **glossary**.

The theme throughout: be curious, not cynical. A short list of
second-long habits — trace the source, zoom, search, read the label —
catches almost every fake aimed at your beliefs, without making you the
person who shouts "AI!!" at real photos.

## A companion, not a repeat

This guide deliberately complements *The AI Scam Safety Guide* (the
money-focused sibling in the same series): AI-written scam messages, fake
profiles and listings, cloned-voice *phone calls* and the family
passphrase, fake AI tool sites, too-good deals, verifying people and
payments, and recovery after dollars left the account all live **there**;
here the focus is fake *media* aimed at what you believe — wherever it
shows up, from memes to news to the group chat. The two handbooks
cross-reference instead of re-teaching each other.

## Who's behind it

Written and maintained by **Asdale Dynamics, LLC** as part of its
beginner-friendly guide series — the same spirit behind the book
*The Massive AI Manual*: plain English, step by step, warm, never
condescending, never alarmist.

## Read it

The Markdown "source of truth" lives in [`docs/`](docs/). Build the static
site and open it in any browser:

```bash
python3 build.py
```

That generates `site/` — a self-contained static HTML site with no external
dependencies, no analytics, no cookies, and no JavaScript requirement (one
optional print button for the checklist). Open `site/index.html` to start
reading. Everything works offline.

## Test it

```bash
python3 -m unittest discover -s tests -v
```

The suite covers the Markdown-to-HTML converter (headings, anchors, lists,
task lists, tables, quotes, code fences, callouts, expandable details,
inline formatting, link rewriting), an end-to-end build into a temporary
directory, internal link and anchor checking, the required copyright line
in every page footer, and a scan for secret-shaped strings in repo files.

`build.py` also verifies every internal link and anchor after each build
and exits non-zero on a problem, so a broken cross-reference can't ship
quietly.

## Repo layout

```
docs/          14 Markdown pages (the source of truth)
assets/        style.css + favicon.svg (copied into the site at build)
build.py       stdlib-only Markdown → static HTML builder + link checker
tests/         unittest suite (converter + end-to-end + repo checks)
site/          generated output (not committed; run python3 build.py)
```

## License

MIT — see [`LICENSE`](LICENSE). Copyright (c) 2026 Asdale Dynamics, LLC.
