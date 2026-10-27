# STATUS — The Spot Fake Media Guide

Built: 2026-10-27 · Owner: Asdale Dynamics, LLC

## What was built

A complete beginner's manual for spotting fake media, delivered as both
readable Markdown and a self-contained static HTML site. Warm, plain-English,
local-first, no jargon.

- **`docs/` — 14 Markdown pages (the source of truth):**
  - `index.md` — start-here intro, the "believe less, verify more" calm
    promise, the route table, and explicit companion rules vs. *The AI Scam
    Safety Guide* (media side here, money side there; cross-referenced by
    name, never re-taught).
  - `01` what changed and why screens need checking now (free generation,
    enormous distribution, dead old tells; where fakes actually show up;
    the "shallowfake"; the crying-wolf problem and how the guide avoids it).
  - `02` AI-made images and the zoom-in habit (eight ordered tells: hands,
    text, reflections, light logic, background melt, texture, seams,
    teeth/eyes; what real photos look like; a verdict ladder table).
  - `03` fake screenshots (eight seam-reading checks; pasted-line seams,
    clock math, handle fingerprints, "forwarded many times"; payment
    "receipts" delegated to the scam guide; the phone workflow).
  - `04` cloned voices and "leaked audio" (listening tells: breath, the
    0.5x pause test, prosody, word salad, room sound, join seams; the
    un-Googleable question; the second-source rule; a genre table; live
    phone-call defense delegated to the scam guide).
  - `05` deepfake video (seven watch-tells in order incl. lip-sync on
    P/B/M and face-edge seams; the slow-motion trick; the keyframe move;
    shallowfake questions; a "before you accuse" guardrail).
  - `06` reverse image search step by step (Google Lens / TinEye / Bing /
    Yandex on phone and desktop; the oldest-first reading habits; crop
    search; privacy guardrails; the video keyframe recap).
  - `07` provenance: C2PA / Content Credentials in plain English (what the
    receipt trail shows; contentcredentials.org/verify; Meta/YouTube
    labels; SynthID invisible watermarks; a five-line honest-limits table).
  - `08` ask AI to check AI (three prompt recipes: tell-spotter,
    source-tracer, outrage-meter; detector unreliability; hallucinated
    tells; the "what would change your mind" habit; privacy guardrails).
  - `09` family group chats (the three-question pause; forwarding hygiene;
    four kind reply scripts; the two conversations not to have in the chat).
  - `10` the calm playbook (the seven-step five-minute loop with times; a
    four-verdict table where "unresolved" is legitimate; low-energy
    versions of the loop).
  - `11` practice scenes (five realistic little mysteries with expandable
    answers, plus a family drill for inventing your own set).
  - `checklist.md` — printable checklist (36 checkboxes, print button,
    print-friendly CSS).
  - `glossary.md` — 22 plain-English terms, alphabetical, with chapter
    pointers.
- **`build.py`** — stdlib-only Markdown → static HTML builder (headings
  with anchors, lists, task lists, tables, quotes, code fences, callouts,
  expandable `<details>` answers, inline formatting, `.md` → `.html` link
  rewriting, prev/next nav, shared header/footer). After every build it
  runs an internal link/anchor checker and exits non-zero on any problem.
- **`assets/`** — hand-written `style.css` (warm paper theme, responsive,
  print rules) and `favicon.svg` (magnifier). No external assets, no CDN,
  no fonts fetched, no JavaScript beyond one optional print button.
- **`site/`** — generated output (gitignored; rebuild with
  `python3 build.py`).
- **`tests/test_build.py`** — 35 tests: converter units (including the
  callout/details extensions and error cases), end-to-end build into a
  temp dir, page/anchor resolution, footer copyright checks, README/License
  checks, practice-answer hidden-details check, local-first assertions, and
  a secret-shaped-string scan of repo files.

## How to run it

```bash
python3 build.py                          # build site/ + link check
python3 -m unittest discover -s tests -v  # run the 35 tests
```

Then open `site/index.html` in any browser. Everything works offline;
`site/` is self-contained. Python 3.10+ (developed on 3.13); no packages
to install.

## Verification results

- `python3 build.py` → **Built 16 files** (14 HTML pages + style.css +
  favicon.svg); **link check OK: 14 pages, all 264 hrefs resolve**
  (internal links and anchors).
- `python3 -m unittest discover -s tests` → **Ran 35 tests … OK**.
- Every built page parses as well-formed HTML (tag-balance check via
  Python's `html.parser`); nav carries all 14 chapters on every page;
  checkbox list renders 36 tasks on the checklist; the five practice
  answers render as hidden `<details>`.
- `LICENSE` contains the exact line `Copyright (c) 2026 Asdale Dynamics,
  LLC`; `README.md` credits Asdale Dynamics, LLC; every page footer
  carries the same copyright line (all three are test-asserted).
- Git: initialized on `main`, single plain commit with the existing git
  identity, no co-author trailers, no remote, nothing pushed. `site/` is
  gitignored by design (regenerable output).

## Known gaps

- **No real sample media.** Practice scenes are described in prose rather
  than shipped as example images/audio/video — deliberate (local-first, no
  binary assets, nothing that could be mistaken for real harmful media),
  but a future "sample files" pack with synthetic images could add a
  hands-on layer.
- **Detection reality.** No method in the guide (human or AI) is reliable
  against the newest generators; the guide says so plainly and leans on
  source-tracing and provenance instead. Specific tool UIs (Lens, TinEye,
  platform AI labels) change constantly; the pages teach the *shape* of
  each check.
- **English only**; a large-print/translated variant could widen reach.
- **C2PA tooling is young** — the verify flow works today, but labels,
  detectors, and platform naming keep shifting; the stable concepts are
  what the chapter teaches.
- The guide is education only — not legal, medical, or financial advice;
  money-shaped situations are handed off to *The AI Scam Safety Guide*.
