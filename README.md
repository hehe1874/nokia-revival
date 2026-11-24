# Nokia Revival — a feature phone in the browser

**Kiroween 2026 · Resurrection track · Solo · Jian Liu (17173sd)**

Bring a Nokia-style feature phone back to life as a web app: the chunky
plastic body, the T9 keypad, Snake, and a ringtone composer — all running
in the browser, no install.

## What it does (planned)

- **Phone shell** — pixel screen, physical-feel keypad, D-pad navigation.
- **T9 texting** — multi-tap / predictive input on the 2–9 keys, just like
  the originals.
- **Snake** — the classic, playable with the D-pad / arrow keys.
- **Ringtone composer** — tap out a melody on the keypad, play it back
  with WebAudio, save it.

## Run it

Open `index.html` in a browser. No build step, no server needed.

## Tech

Plain HTML + CSS + JavaScript. No framework — the point is the
resurrection, not the toolchain. Built with Kiro (`.kiro/` holds the
specs and steering docs Kiro works from).

## Submission

- Hackathon: Kiroween 2026 (Devpost), category **Resurrection**
- Devpost profile: https://devpost.com/17173sd
- Public repo rule: the repo root must contain a `/.kiro` directory
  (per Devpost's "Keep the Momentum Going" email, 2026-11-12 00:35
  Beijing) — this skeleton already has it.
- Submit by **2026-12-05 06:00 Beijing**. See `TIMELINE.md`.

## Status

Shell + menu done; **Snake playable since 2026-11-12** (D-pad / arrow
keys, score + best, game over, OK to retry, # back to menu). **Messages +
multi-tap T9 done 2026-11-13**, and **ringtone composer done 2026-11-13**
(1–9 = C4–D5 notes, 0 = rest, OK plays the melody, ↑↓ tempo, saved in
localStorage). **Polish done 2026-11-13** (key-click sounds, press and
screen-swap animations, food blink, small-screen layout). Only submission
packaging (task 7) remains.
See `.kiro/specs/nokia-phone/tasks.md` for the build order.
