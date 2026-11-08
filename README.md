# Lights; low — Diatonic Crime

A small MIDI chord generator for REAPER. Press one MIDI key and it generates
up to four notes chosen by scale degree.

It is useful for quickly playing diatonic triads, sevenths, add-nine chords,
power chords, and deliberately questionable extended voicings.

## Features

- Choose a tonic from C through B.
- Major, Natural Minor, Dorian, Mixolydian, Phrygian, Lydian, Locrian, and
  Chromatic scales.
- Toggle degrees 1, 2, 3, 5, 7, and 9.
- Generates up to four notes per input note.
- Outside-scale roots can be allowed, rounded down, or blocked.
- Output octave and semitone transpose controls.
- Correctly tracks generated note-off messages.
- Pass-through options for other MIDI messages.
- One dependency-free JSFX file.

## Install

1. In REAPER, choose **Options > Show REAPER resource path in explorer/finder**.
2. Open the `Effects` folder.
3. Copy `Diatonic Crime` into that folder or a subfolder.
4. Restart REAPER or refresh the FX browser.
5. Add **JS: Diatonic Crime** before a virtual instrument.

## Use

Select a tonic and scale, then enable the desired scale degrees.

Examples:

| Enabled degrees | Result |
| --- | --- |
| 1, 3 | Third shell |
| 1, 5 | Power chord |
| 1, 3, 5 | Triad |
| 1, 3, 7 | Open seventh voicing |
| 1, 3, 5, 7 | Seventh chord |
| 1, 3, 5, 9 | Add-nine chord |
| 1, 3, 7, 9 | Extended shell voicing |

If more than four degrees are enabled, the lowest four are used.

### Roots outside scale

- **Allow:** use the played note as a chromatic root.
- **Round down:** move it to the nearest scale note below.
- **Block:** do not generate a chord.

For example, with D Natural Minor and **Round down** selected, F-sharp becomes
F, B becomes B-flat, and C-sharp becomes C.

## License

Personal and noncommercial use is free.

For commercial music or audio use, choose either:

- Use it free and include **“Diatonic Crime by Carl Kashnier”** in the
  album, release, or project credits.
- Pay **$5 USD once per person or business** and no credit is required. Pay
  through PayPal to **CarlKashnier@gmail.com** and include
  `Diatonic Crime commercial license` in the payment note.

There are no royalties on anything you make with the plugin. Selling,
bundling, or commercially redistributing the plugin itself requires separate
written permission. See [LICENSE](LICENSE) for the complete terms.

