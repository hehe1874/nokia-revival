# Design — Nokia phone in the browser

## Look

- Classic candybar: dark grey-blue body, rounded corners, small
  landscape-feel screen (roughly 4:3), green-tinted LCD look.
- Pixel-style font for the screen; monospace fallback so it renders
  anywhere.
- Keypad: 3×4 grid, slightly raised buttons, press animation.

## Screen

- 240×320 logical pixels, scaled up with `image-rendering: pixelated`
  for canvas elements.
- Home screen: status bar (signal bars, battery), clock, menu list.
- One screen at a time; softkeys are Back / Select.

## Snake

- Canvas grid, e.g. 20×28 cells; snake moves one cell per tick.
- Tick interval starts ~150 ms, shortens as the snake eats.
- Food spawns on a random free cell; score +10 per food.

## Audio

- WebAudio oscillator (square wave) for key beeps and notes.
- Composer: keys 1–7 map to a C-major scale; 0 = rest, # = octave up.
- Playback schedules notes with `AudioContext` timing, not `setTimeout`
  chains.

## Files

- `index.html` only, until it outgrows one file. CSS in `<style>`,
  JS in `<script>` at the end of body.
