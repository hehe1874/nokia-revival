# Tasks — build order

- [x] 1. Phone shell: body, screen, keypad grid, D-pad, softkeys (R1–R3)
- [x] 2. Home screen: status bar, clock, menu navigation (R2–R3)
- [x] 3. Messages + multi-tap T9 input (R4–R5) — done 2026-11-13, ahead of the Nov 19–21 slot; verified in a headless run (multi-tap cycling, 900 ms timeout commit, 0=space, 1=punct, backspace, OK sends to Sent, inbox/read navigation)
- [x] 4. Snake: canvas, movement, food, score, game over (R6–R7) — done 2026-11-12, ahead of the Nov 17–18 slot; verified in a headless run (eat +10 and grow, steer, wall/self game over, OK restarts)
- [x] 5. Ringtone composer: note mapping, WebAudio, save/load (R8–R10) — done 2026-11-13, ahead of the Nov 22–24 slot; verified in a headless run (1–9 notes C4–D5, 0=rest, OK plays whole melody, ↑↓ tempo 60–240 BPM, * deletes, 32-note cap, localStorage save/reload, Snake + T9 regression pass)
- [x] 6. Polish: key-press sounds, animations, small-screen layout — done 2026-11-13, ahead of the Nov 25 slot; verified in a headless run (key click via WebAudio on dpad/select/keypad except composer notes, .pressed flash on the matching button, screen-swap fade, food blink, no regressions in Snake/T9/composer)
- [ ] 7. Submission: README final pass, screenshots, Devpost form (R11–R13)

Work top-down; each task should leave the app runnable.
