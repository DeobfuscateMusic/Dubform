<p align="center"><img width="210" height="164" alt="dubformbanner" src="https://github.com/user-attachments/assets/33318e27-2958-4e98-a061-d375c6bdd379" /></p>

**_<p align="center">Dub Techno 12-bit Sampler & Tape Delay.</p>_**

---

![Version](https://img.shields.io/badge/Version-1.1.0-brightgreen?style=flat-square)
![macOS Support](https://img.shields.io/badge/macOS-Sonoma%20%7C%20Sequoia%20%7C%20Tahoe-000000?style=flat-square&logo=apple&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Universal-black?labelColor=606060&style=flat-square&logo=apple&logoColor=white)
![Format](https://img.shields.io/badge/Format-Standalone-00CED1?style=flat-square)
![DAW](https://img.shields.io/badge/DAW-Ableton%20Live%2012%2B-000000?style=flat-square&logo=abletonlive&logoColor=white)

---

<img width="996" height="788" alt="dubformpreview" src="https://github.com/user-attachments/assets/23bcf855-2c19-4dda-9864-75de009603ac" />

---

## 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬

- **Variable Bit-Depth Sampler**: Reduces the bit resolution of the incoming signal from 16 bits down to 2, introducing digital quantization noise, crunch, and the characteristic texture of vintage samplers and early digital hardware.
- **Clock Rate Downsampling**: Lowers the effective sample rate from 44.1 kHz down to 6 kHz, producing aliasing artefacts and the gritty, lo-fi character associated with SP-1200 and early Akai hardware.
- **Multi-Mode Filter**: A biquad filter with four modes — Lowpass, Bandpass, Highpass, and Notch — with resonance control and an analog-style soft-clipping drive stage. Gain compensation is applied automatically to prevent volume jumps as drive increases.
- **Tape Echo**: A delay unit with adjustable delay time and feedback intensity, plus a wow/flutter LFO that modulates the delay time to simulate the pitch instability of vintage tape delay machines such as the Roland RE-201.
- **8 Dub Techno Presets**: Named configurations covering a range of classic dub and dub techno processing approaches, from clean deep space echo to heavily degraded lo-fi textures.
- **Live Output Recording**: Captures the processed master output directly to a stereo 16-bit WAV file, timestamped and downloaded automatically.
- **VU Meter**: Vintage-style analog meter with mechanical ballistic simulation — fast attack, weighted release — for monitoring output levels.
- **Waveform Display**: Visual representation of the loaded audio with a real-time playhead. Click or drag to seek to any position in the sample.
- **Offline Operation**: All processing runs locally. No network access required during use.

---

## 𝐒𝐲𝐬𝐭𝐞𝐦 𝐑𝐞𝐪𝐮𝐢𝐫𝐞𝐦𝐞𝐧𝐭𝐬

- **macOS**: 14.0 (Sonoma), 15.0 (Sequoia) or 16.0 (Tahoe)
- **Architecture**: Intel (x64), Apple Silicon (Arm64) or Universal (U2B)
- **RAM**: 256 MB minimum
- **DAW (Plugin mode)**: Ableton Live 12 or 11, Logic Pro, Reason with the [BlackHole](https://github.com/ExistentialAudio/BlackHole) virtual audio driver for DAW routing in standalone mode.
> Audio Unit (AU) & VST3 plugins formats are currently under development.

---

## 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧

### 𝐒𝐭𝐚𝐧𝐝𝐚𝐥𝐨𝐧𝐞

1. Download the latest [`Dub Stabs`](https://github.com/KouseiMusic/Dub-Stabs/releases/download/Dub_Stabs_1.1.0/Dub.Stabs.macOS.Universal.zip).
2. Extract & Drag `Dub Stabs` to your `Applications` folder.
3. If macOS shows a Gatekeeper warning on first launch, right-click the application and choose `Open`, then confirm.

### 𝐀𝐮𝐝𝐢𝐨 𝐔𝐧𝐢𝐭 (𝐀𝐔)

> 𝐔𝐧𝐝𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭

### 𝐕𝐒𝐓𝟑

> 𝐔𝐧𝐝𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭

## 𝐃𝐀𝐖 𝐔𝐬𝐚𝐠𝐞

1. Install [`BlackHole`](https://github.com/ExistentialAudio/BlackHole), a free virtual audio driver for macOS.
2. Open `Audio MIDI Setup` (found in `/Applications/Utilities/`).
3. Create a `Multi-Output Device` that includes both your `Audio Interface` and `BlackHole`.
4. Set the `Multi-Output Device` as the system output in `System Settings` > `Sound`.
5. In your `DAW`, create an `Audio Input Track` and set its input source to `BlackHole`.
6. You can now record or monitor `Dubform`'s output in real time.

---

## 𝐒𝐢𝐠𝐧𝐚𝐥 𝐂𝐡𝐚𝐢𝐧

```
┌─────────────────────────────────────────────────────────────────────────┐
│                           DUBFORM SIGNAL PATH                           │
└─────────────────────────────────────────────────────────────────────────┘

  AUDIO FILE
  (WAV / AIFF / MP3 / AAC / FLAC)
       │
       ▼
┌─────────────┐
│   SAMPLER   │  Bit Depth (2–16 bit) - reduces resolution / adds crunch
│             │  Clock Rate (6–44.1kHz) - slows the clock / adds aliasing
└──────┬──────┘
       │
       ▼
┌─────────────┐
│    DRIVE    │  Soft-clipping saturation stage before the filter.
│ (pre-filter │  Pushes the signal into harmonic warmth without hard
│ saturation) │  Distortion. Gain compensation applied automatically.
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   FILTER    │  Mode: LP / BP / HP / NOTCH
│             │  Cutoff (20 Hz - 20 kHz) - sets the Frequency point.
│             │  Resonance (0.0 - 1.0) - emphasises the Cutoff peak.
└──────┬──────┘
       │
       ├──────────────────────────────────────┐
       │                                      │
       ▼                                      ▼
  (Dry Path)                        ┌─────────────────────────────────┐
       │                            │     TAPE ECHO                   │
       │                            │  Rate (delay time)              │
       │                            │  Intensity (feedback, max 0.93) │
       │                            │ Wow/Flutter (tape pitch wobble) │
       │                            │        ┌────────────────────────┘
       │                            │        │
       │                            │        │
       │                            │    ┌───┴────┐
       │                            │    │FEEDBACK│ ◄── Self-Loop
       │                            │    │  LOOP  │    (Hard-Limited
       │                            └────┤        │     below 1.0)
       │                                 └───┬────┘
       │                                     │
       ▼                                     ▼
┌─────────────────────────────────────────────────┐
│                  MASTER OUTPUT                  │
│              Volume (0-200%)                    │
└───────────────────────┬─────────────────────────┘
                        │
           ┌────────────┼──────────────┐
           ▼            ▼              ▼
     AUDIO OUTPUT   VU METER       RECORDER
                 
```

---

## 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

### 𝐒𝐚𝐦𝐩𝐥𝐞𝐫

The sampler section degrades the incoming audio to simulate vintage digital hardware. Both controls affect the playback engine directly and update in real time.

| Control | Description | Range |
| :--- | :--- | :--- |
| **Bit Depth** | Reduces the resolution of the audio signal. Lower values introduce pronounced quantization noise and a gritty, textured crunch. Values above 12 are relatively clean; below 8 the degradation becomes a strong character in itself. | 2 to 16 bit |
| **Clock** | Reduces the effective sample rate by slowing playback and re-pitching. Lower values produce aliasing, artefacts, and the distinctive texture of hardware with a low clock speed. 44.1 kHz is unprocessed; 6 kHz is maximum degradation. | 6 kHz to 44.1 kHz |

### 𝐅𝐢𝐥𝐭𝐞𝐫

| Control | Description | Range |
| :--- | :--- | :--- |
| **Cutoff** | The frequency at which the filter begins to attenuate the signal. In Lowpass mode this rolls off the high end; in Highpass it attenuates the lows; in Bandpass it isolates a frequency region around this point. | 20 Hz to 20,000 Hz |
| **Resonance** | Boosts the signal at and immediately around the cutoff frequency, adding emphasis and, at higher settings, a characteristic ringing or whistling peak. Gain compensation reduces the overall level as resonance increases to prevent harsh spikes. | 0.0 to 1.0 |
| **Drive** | Pushes the signal through a soft-clipping waveshaper before it enters the filter. Adds harmonic saturation and analog-style warmth. Automatic gain compensation is applied so the perceived volume remains consistent as drive increases. | 1x to 10x |
| **Mode** | Selects the filter topology. **LP** (Lowpass) passes frequencies below the cutoff and is the most common mode for dub-style dark filtering. **BP** (Bandpass) isolates a frequency band, useful for telephony and formant effects. **HP** (Highpass) removes low frequencies. **NOTCH** creates a narrow dip at the cutoff, producing a phaser-like sweep when automated. | LP / BP / HP / NOTCH |

### 𝐄𝐜𝐡𝐨

The echo section models a tape delay unit.

| Control | Description | Range |
| :--- | :--- | :--- |
| **Rate** | The time between the original signal and its first delayed repeat. Short times (under 200 ms) produce slap-back and rhythmic doubling. Longer times (400 ms and above) produce classic dub echo and spatial wash effects. | 0.01 s to 2.0 s |
| **Intensity** | How much of the delayed signal is fed back into the delay input, controlling the number of audible repeats. At low values the echo fades quickly; at high values it sustains into a long, slowly-decaying tail. The maximum value (0.93) approaches but never reaches infinite feedback. | 0.0 to 0.93 |
| **Wow / Flutter** | Applies a slow LFO to the delay time, simulating the pitch instability caused by motor irregularities and tape speed variation in analog tape machines. At low values this adds subtle warmth and movement; at higher values the pitch modulation becomes an audible, swaying wobble. | 0.0 to 1.0 |

### 𝐆𝐥𝐨𝐛𝐚𝐥 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

| Control | Description |
| :--- | :--- |
| **Load** | Opens a file dialog to select and load an audio file. Playback begins automatically once the file has decoded. |
| **Presets** | Dropdown menu with 8 preset configurations covering a range of dub and dub techno processing approaches. Selecting a preset applies all sampler, filter, and echo parameters simultaneously with a brief smoothing transition to prevent clicks. |
| **Volume** | Master output gain, controlling the level of the final signal sent to the audio output. The default is 80%. Values above 100% provide additional gain for quieter source material. |
| **Record** | Starts and stops live recording of the master output. When stopped, the captured audio is written as a stereo 16-bit WAV file and downloaded automatically. The filename includes the date and time of the recording. |
| **Play** | Starts playback of the loaded sample from the current playhead position. |
| **Pause** | Pauses playback and holds the playhead at the current position. Pressing Play resumes from where it was paused. |
| **Stop** | Stops playback and returns the playhead to the beginning of the sample. |
| **Waveform** | The waveform panel at the bottom of the interface displays the loaded audio. Click anywhere on the panel to jump to that position, or click and drag to scrub through the sample in real time. |

---

## 𝐏𝐫𝐞𝐬𝐞𝐭𝐬

| Preset | Character |
| :--- | :--- |
| **Classic Dub** | Warm 12-bit degradation, short echo with moderate feedback. Evokes the classic Roland Space Echo processing of Jamaican dub production. |
| **Deepchord Space** | Clean 16-bit signal, long dark delay, deep lowpass filtering. Characteristic of the vast, oceanic textures of mid-2000s Detroit dub techno. |
| **Submerged** | Heavy 8-bit crush and low clock rate, deep sub-100 Hz filter, medium delay. Dense and claustrophobic. |
| **Resonant Drift** | 12-bit signal through a bandpass filter with controlled resonance. The narrow frequency band and drifting echo produce a hypnotic, cycling texture. |
| **Infinite Wash** | Clean 16-bit source through a bright lowpass with high feedback. Creates a slowly building, enveloping ambient wash. Feedback is held just below the sustained ceiling. |
| **Basic Channel** | 12-bit signal, tight lowpass, medium delay with sustained feedback. References the minimal, stripped-back aesthetic of Maurizio and early Basic Channel releases. |
| **Night Drive** | 24-bit clean signal through a gentle filter with short, quiet echo. Transparent and unobtrusive — useful as a starting point or for subtle processing. |
| **Echospace Tape** | 10-bit degradation, mid-range lowpass, long tape echo with pronounced wow flutter. Heavy and worn, referencing the saturated tape aesthetic of Echospace and Intrusion releases. |

---

## 𝐑𝐞𝐜𝐨𝐫𝐝𝐢𝐧𝐠

Press the `Rec` button to begin capturing audio. Press it again to stop. A `.wav` file is exported automatically and named using the active preset abbreviation and the current date and time (e.g. `dubform_260609143022.wav`). Recording captures the full processed signal including delay, reverb and the master limiter.

---

_This software is free. If you find it useful, a star on GitHub is appreciated._

---

<p align="center"><code>Kousei</code></p>
<p align="center">2026</p>
