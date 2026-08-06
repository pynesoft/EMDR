# EMDR — Master Mode

A single-file, browser-based EMDR (Eye Movement Desensitization & Reprocessing) tool with a twist: **Master Mode**, an experimental right-hemisphere "awakening" phase inspired by Iain McGilchrist's *The Master and His Emissary*.

No install, no build step, no server, no tracking. One HTML file. Open it and go.

## Features

### Standard EMDR
- Smooth bilateral sweep with adjustable speed, travel width, and tap tempo
- Dot styles (sphere, flat, ring, cross), colors, size, motion trail, and bounce flash
- Timed sessions (1–20 min) or unlimited
- Settings auto-save to your browser (localStorage only — nothing leaves your machine)

### Master Mode
Named for McGilchrist's "Master" — the right hemisphere. Because each hemisphere processes the *opposite* visual field and ear, Master Mode opens every session with an **Awakening phase** that feeds stimulation to your left side:

- The dot drifts **right to left only**, fading out at the left edge and reappearing on the right
- Audio pans **hard to the left ear**
- A 1980s-style wireframe depth field appears — horizon, vanishing point, and a tracking ray that follows the ball — an implicit spatial-depth cue the right hemisphere is thought to specialize in
- After a set time (30 sec – 5 min), an A-minor arpeggio chimes and the session transitions into standard bilateral EMDR

### Audio Engine
Three sound modes, all with optional binaural beat (per-voice detune between ears) and bilateral panning:

| Mode | Voices | Character |
|---|---|---|
| Pure Tone | root only | Classic binaural sine |
| Harmonics | root · fifth · octave · 12th | Warm natural overtone stack |
| Minor Chord | root · 6/5 · 3/2 (just intonation) | Smooth minor triad — A–C–E at the default 220 Hz root |

## Install (PWA)

The app is installable and works offline once loaded.

- **Desktop Chrome/Edge:** click the install icon in the address bar, or the **Install App** button in the app
- **Android Chrome:** menu → *Add to Home screen*
- **iOS Safari:** Share → *Add to Home Screen*

Installed, it launches in its own window with no browser chrome and runs without a connection.

## Screen & Display

- **Keep screen awake** — uses the Screen Wake Lock API so your display won't dim or sleep mid-session (on by default; Chrome, Edge, and Android — Safari support varies)
- **Fullscreen** — button, or press `F`. Hides all controls except Start/Stop and scales the canvas to fill the screen
- **Auto fullscreen** — optional toggle in the Session tab to enter fullscreen whenever a session starts

## Usage

1. Download `index.html` (or clone the repo)
2. Open it in any modern browser
3. Put on headphones
4. Optionally toggle **Master Mode**, then **Start Session**

Tip: for the smoothest chord, set the binaural beat to 0 — just intonation with no detune has almost no roughness.

## Disclaimer

This is a personal experiment, not a medical device, and not a substitute for therapy. EMDR is normally done with a trained clinician; self-administered bilateral stimulation can surface difficult material. The hemisphere-activation premise behind Master Mode is drawn from McGilchrist's framing of hemispheric lateralization and is **not** an established clinical technique. Use at your own discretion, and stop if you feel worse. If you have a therapist, tell them you're using it.

Do not use while driving or operating anything. Flashing/moving visuals may affect people with photosensitive conditions.

## License

[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) — free to use, share, and adapt for non-commercial purposes with attribution.

A [pynesoft](https://github.com/pynesoft) project.
