# 𝐃𝐮𝐛𝐟𝐨𝐫𝐦 - 𝐂𝐡𝐚𝐧𝐠𝐞𝐥𝐨𝐠

## 𝟏.𝟏.𝟎 (𝟎𝟔-𝟐𝟎𝟐𝟔)

### 𝐒𝐨𝐮𝐧𝐝 & 𝐏𝐞𝐫𝐟𝐨𝐫𝐦𝐚𝐧𝐜𝐞

- Fixed audio dropouts and stuttering during recording. The previous recording system ran on the same thread as the rest of the application, meaning brief spikes in CPU activity from moving knobs or opening menus could interrupt the audio stream. The recorder has been moved to a dedicated audio thread, isolating it from interface activity for glitch-free captures.

- Fixed a volume jump when starting a recording. The recorder was previously wired into the output path in a way that added a second copy of the signal to the speakers, causing a noticeable boost in level. The recorder now listens to the signal passively without contributing to the output, ensuring consistent monitoring levels.

- Fixed echo feedback running away under high intensity settings. At extreme values, repeats were able to build indefinitely rather than decaying, resulting in an uncontrolled, escalating wall of sound. A hard limit is now enforced at all times, ensuring every echo tail eventually fades out regardless of knob position.

- Fixed clicks and pitch glitches when adjusting echo controls while Wow/Flutter was active. The tape-wobble effect and delay time adjustments were competing for control over the sample rate, producing audible artifacts. The modulation now smoothly steps back while the echo settles into a new setting before fading back in.

- Fixed the Drive knob not responding correctly when switching filter modes. The internal recalculation required to match the drive circuit to different tonal characters (Lowpass, Bandpass, etc.) was occasionally being skipped. The drive behavior now updates immediately and accurately every time a filter mode is changed.

- Fixed audio resources not being released when loading new files. Previous engine instances, including oscillators and processing nodes, were being left running silently in the background after a new file was loaded. The engine is now fully shut down and its memory cleared before a new session begins.

### 𝐏𝐫𝐞𝐬𝐞𝐭𝐬

- Recalibrated six presets to prevent clipping and ear fatigue. Several presets reached levels that were too dense for comfortable monitoring or built up too quickly into unmanageable noise. Levels and sustain values have been adjusted to preserve character while keeping the output controllable at normal listening volumes.

- 𝐈𝐧𝐟𝐢𝐧𝐢𝐭𝐞 𝐖𝐚𝐬𝐡: Reduced echo sustain to prevent the tail from building into an unbroken wall of sound; it now reaches a stable plateau.

- 𝐄𝐜𝐡𝐨𝐬𝐩𝐚𝐜𝐞 𝐓𝐚𝐩𝐞: Reduced drive and tape wobble to remove harsh, fatiguing textures while retaining the "worn tape" aesthetic.

- 𝐃𝐞𝐞𝐩𝐜𝐡𝐨𝐫𝐝 𝐒𝐩𝐚𝐜𝐞: Reduced sustain to prevent repeats from masking the original dry signal.

- 𝐑𝐞𝐬𝐨𝐧𝐚𝐧𝐭 𝐃𝐫𝐢𝐟𝐭: Reduced filter resonance and sustain to eliminate unpleasant ringing in the bandpass frequency range.

- 𝐁𝐚𝐬𝐢𝐜 𝐂𝐡𝐚𝐧𝐧𝐞𝐥 & 𝐂𝐥𝐚𝐬𝐬𝐢𝐜 𝐃𝐮𝐛: Slightly reduced echo sustain for better clarity.

### 𝐒𝐞𝐜𝐮𝐫𝐢𝐭𝐲

- Fixed a vulnerability that allowed unauthorized content to run within the application window. A strict policy now prevents any external scripts or malicious files from injecting content into the interface. Additionally, the application now runs in a sandboxed environment to isolate it from the rest of the system.

- Removed an unnecessary third-party package (Express) that was included in the build by mistake. While unused by the application, its presence introduced known security vulnerabilities. Its removal results in a cleaner, more secure installation.

- Fixed the application making unnecessary network requests on startup. The interface was attempting to download fonts from external servers, causing failures on offline systems. The application now uses local system fonts on Sonoma, Sequoia, and Tahoe, requiring no internet access and improving privacy.

- Updated five build-process packages to address known security vulnerabilities. While these tools are not present in the final installed application, updating them ensures a secure and modern development environment.

---

## 𝟏.𝟎.𝟎 (𝟐𝟔-𝟎𝟓-𝟐𝟎𝟐𝟔)

- Variable Bit-Depth Sampler (16-bit down to 2-bit) and Clock Rate Reduction (44.1 kHz down to 6 kHz).

- Multi-Mode Filter (LP, BP, HP, Notch) with Resonance and Drive.

- Tape Echo with adjustable Delay, Feedback sustain, and Wow/Flutter.

- Interactive waveform display with click-to-seek and live VU metering.

- Integrated live recording to stereo WAV and master volume control.

- Native support for macOS Sonoma, Sequoia, and Tahoe (Universal Binary).
