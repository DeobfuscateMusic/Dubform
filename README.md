<p align="center"><img width="312" height="243" alt="Dubform Small" src="https://github.com/user-attachments/assets/e166f0b5-c7a1-4b0a-94eb-203a7c4b1b26" /></p>

_<p align="center">12-bit Sampler for Dub Techno Processing. Combines a tape delay and a lo-fi engine with spatial delays & asymmetrical saturation. Designed specifically for deep textures and atmospheres.</p>_

---

![Version](https://img.shields.io/badge/Version-0.9.9-brightgreen?style=flat-square)
![macOS Support](https://img.shields.io/badge/macOS-Sonoma%20%7C%20Sequoia%20%7C%20Tahoe-000000?style=flat-square&logo=apple&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Universal%20Silicon%20%26%20Intel-black?labelColor=606060&style=flat-square&logo=apple&logoColor=white)
![Format](https://img.shields.io/badge/Format-Standalone%20%7C%20AU%20%7C%20VST3-00CED1?style=flat-square)
![DAW](https://img.shields.io/badge/DAW-Ableton%20Live%2012%2B-000000?style=flat-square&logo=abletonlive&logoColor=white)

---

https://github.com/user-attachments/assets/5829be5e-47bb-4e1f-9735-d871cfe98de1

---

## 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬

- **12-Bit Prophet Engine**: Authentic vintage quantization with variable clock rates (44.1kHz down to 6kHz) for classic aliasing.
- **Tuned Looping**: Advanced sampler logic that forces audio segments to cycle at MIDI-responsive frequencies.
- **Dub Filter**: 4-pole (24dB/oct) State Variable Filter with asymmetrical saturation for analog warmth.
- **Space Echo**: Multi-tap delay with non-linear feedback for sound design.
- **Teal Noir UI**: High-contrast, industrial dark mode interface optimized for precision and low-light focus.
- **Zero Dependencies**: Fully native macOS execution. No external libraries or internet required.

---

## 𝐒𝐲𝐬𝐭𝐞𝐦 𝐑𝐞𝐪𝐮𝐢𝐫𝐞𝐦𝐞𝐧𝐭𝐬

- **macOS**: 14.0 (Sonoma), 15.0 (Sequoia) or 16.0 (Tahoe).
- **Architecture**: Intel & Apple Silicon.
- **DAW**: Ableton Live 11+, Ableton Live 12+, Logic Pro & Reason with [BlackHole](https://github.com/ExistentialAudio/BlackHole) driver.

---

## 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧

### 𝐒𝐭𝐚𝐧𝐝𝐚𝐥𝐨𝐧𝐞
1. Download the latest [`Dubform.zip`].
2. Extract & Drag to your `Applications` folder.
3. Open `Dubform`.
4. Click on `Upload Sample`

### 𝐀𝐮𝐝𝐢𝐨 𝐔𝐧𝐢𝐭 (𝐀𝐔) (𝐀𝐛𝐥𝐞𝐭𝐨𝐧 𝟏𝟐) - 𝐔𝐧𝐝𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭
1. Copy `Dubform.component` to `/Library/Audio/Plug-Ins/Components`.
2. Rescan plugins in Ableton Live 12.
3. Create a MIDI track and load `Dubform` to begin processing

### 𝐕𝐒𝐓𝟑 (𝐀𝐛𝐥𝐞𝐭𝐨𝐧 𝟏𝟐) - 𝐔𝐧𝐝𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭
1. Copy `Dubform.vst3` to `/Library/Audio/Plug-Ins/VST3`.
2. Rescan plugins in Ableton Live 12.
3. Create a MIDI track and load `Dubform` to begin processing.

---

## 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

- **Real-time Audio Processing:** Load any audio sample and manipulate it on the fly.
- **Lo-Fi Sampler Module:** Degrade your audio with variable bit depth reduction and clock rate downsampling.
- **Multi-mode Filter:** Shape the frequency content with Lowpass, Bandpass, Highpass and Notch filters; coupled with an analog-style drive circuit.
- **Tape Echo:** Add space and texture with a delay unit featuring feedback and tape wow/flutter effects.
- **Interactive Waveform Display:** Visualize the loaded audio and click/drag to seek through the sample.
- **VU Meter:** Classic vintage-style stereo VU meter for monitoring output levels.

### 𝐒𝐚𝐦𝐩𝐥𝐞𝐫

| Control | Description | Range |
| :--- | :--- | :--- |
| **Bits** | Reduces the bit depth of the audio, introducing digital quantization noise and crunch. | 2 to 16 Bits |
| **Clock** | Lowers the sample rate, creating aliasing and "ringing" artifacts typical of vintage samplers. | 10% to 100% |

### 𝐅𝐢𝐥𝐭𝐞𝐫

| Control | Description | Range |
| :--- | :--- | :--- |
| **Cutoff** | Sets the frequency point where the filter begins to affect the audio. | 20 Hz to 20,000 Hz |
| **Resonance** | Emphasizes the frequencies right around the cutoff point, creating a peak or "ringing" sound. | 0.0 to 1.0 |
| **Drive** | Pushes the signal into soft-clipping distortion before it leaves the filter. Gain compensation is applied automatically. | 1x to 10x |
| **Mode** | Selects the filter type: Lowpass (**LP**), Bandpass (**BP**), Highpass (**HP**), or Notch (**NOTCH**). | Multi-state |

### 𝐄𝐜𝐡𝐨

| Control | Description | Range |
| :--- | :--- | :--- |
| **Repetitions** | Sets the delay time between successive echo repeats. | 0.0s to 1.0s |
| **Feedback** | Controls how much of the delayed signal is fed back into the delay line, determining the number of repeating echoes. | 0.0 to 0.9 |
| **Width (Wow)** | Introduces a slow, randomized pitch fluctuation simulating the wow and flutter of a vintage analog tape delay. | 0.0 to 1.0 |

### 𝐆𝐥𝐨𝐛𝐚𝐥 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

| Control | Description |
| :--- | :--- |
| **Upload Sample** | Opens a file dialog to select and load a new audio file (most standard audio formats are supported). |
| **Play** | Starts playback of the loaded sample. |
| **Pause** | Pauses playback at the current position. |
| **Stop** | Stops playback and returns the playhead to the beginning of the sample. |
| **Waveform** | Click and drag along the waveform panel to scrub / seek through the audio in real-time. |

---

_This software and plugins are free. Don't forget to give it a ⭐ on Github if you liked the project._

---

<p align="center"><img width="91" height="78" alt="Logo_Deobfuscate_RoundXS" src="https://github.com/user-attachments/assets/bc520a4f-d36b-45e3-8e00-c2b928b4f449" /></p>
<p align="center"><code>𝕯𝖊𝖔𝖇𝖋𝖚𝖘𝖈𝖆𝖙𝖊</code></p>
<p align="center">2026</p>
