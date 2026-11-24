# Structure

```
.
├── index.html                  # the whole app (single file, no build)
├── README.md
├── TIMELINE.md                 # reverse schedule to 2026-12-05 06:00
├── LICENSE                     # MIT
└── .kiro/
    ├── steering/
    │   ├── product.md          # what this is and why
    │   └── structure.md        # this file
    └── specs/
        └── nokia-phone/
            ├── requirements.md # what "done" means per feature
            ├── design.md       # screen, keypad, game, audio design
            └── tasks.md        # build order, checkboxed
```

## Conventions

- One file for the app (`index.html` + inline CSS/JS) until it gets
  too big to hold in one head — then split JS into `app.js`, never
  into a bundler.
- All state lives in plain JS objects; no storage dependency except
  `localStorage` for saved ringtones / high score.
- Keyboard: arrow keys = D-pad, digits = keypad, Enter = select.
- Keep it dependency-free so the Devpost demo link works anywhere.
