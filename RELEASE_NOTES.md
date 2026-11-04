# Cherry Buzz 1.0.0

First public release of Cherry Buzz, a free tempo-synced multi-effect by
Oleh Cherkes / Cherry (UA).

## Features

- **BUZZ**: one master knob that drives the whole effect chain (0 % dry to 100 %).
- **FILTER**: 24 dB/oct DJ low-pass / high-pass over 20 Hz – 20 kHz, with RESO.
- **CRUSH**: bit-depth and sample-rate reduction.
- **GATE**: tempo-synced stutter gate, 1/4 – 1/32 steps, adjustable open/closed ratio.
- **NOISE**: noise riser that feeds the reverb and rises in level and brightness.
- **DELAY**: tempo-synced, 1/64 note to 1 bar, with ping-pong.
- **REVERB**: from a room to a ~100 s tail.
- **LOW SAFE**: keeps the bass below 120 Hz out of the effects.
- 12 factory presets, including Build Up Soft / Wild for drops; user presets (save, import, export).
- RMS input / output meters with clip indicators, smooth bypass, 75–200 % window size.
- Zero latency; mono and stereo.

## Downloads

| File | System |
|---|---|
| `Cherry-Buzz-v1.0.0-Windows-x64.zip` | Windows 10+ 64-bit, Intel / AMD (VST3) |
| `Cherry-Buzz-v1.0.0-Windows-ARM64.zip` | Windows on ARM, native ARM64 DAWs (VST3) |
| `Cherry-Buzz-v1.0.0-macOS-Universal.zip` | macOS 10.13+ Intel and macOS 11+ Apple Silicon (VST3 + AU) |

`SHA256SUMS.txt` lists the SHA-256 checksum of every archive.

## Installation

- **Windows**: copy `Cherry Buzz.vst3` to `C:\Program Files\Common Files\VST3\`, then rescan plugins in your DAW.
- **macOS**: copy `Cherry Buzz.vst3` to `~/Library/Audio/Plug-Ins/VST3/` and `Cherry Buzz.component` to
  `~/Library/Audio/Plug-Ins/Components/`, then restart your DAW.

Each archive contains `INSTALL.txt` with step-by-step instructions.

## Known limitations

- The macOS build is not notarized by Apple. If macOS blocks the plugin, allow it in
  **System Settings › Privacy & Security › Open Anyway** (see INSTALL.txt). There is no need to
  disable Gatekeeper.
- The Windows ARM64 build is for DAWs running natively on ARM64; x64 DAWs on Windows on ARM
  need the x64 build.
- There is no output or mix knob: DELAY and REVERB add their wet signal on top of the dry one,
  so high settings get louder — watch your channel level.
- At 100 % the reverb rings for about 1.5 minutes; leave room at the end when you export.
- The meters show the RMS level, so a peak meter in your DAW will read higher.
