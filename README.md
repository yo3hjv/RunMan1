# RunMan I — Music Player for M5Stack TAB5

RunMan I is a touch-friendly, dual-core music player built for the **M5Stack TAB5**.
It scans your SD card library, displays a track list, and plays common audio formats with real-time meters and tone controls.

## Highlights

- **SD card library scan**
  - Automatically scans the **`/Music`** folder on the SD card.
- **Multi-format playback**
  - Plays: **MP3**, **WAV**, **FLAC**, **AAC**, **OGG** (depending on decoder support).
- **Smooth, responsive UI**
  - Large on-screen track list with touch interaction.
  - On-screen playback controls.
- **Dual-core architecture**
  - Audio runs on a dedicated task (Core 0).
  - GUI and touch handling run on the main loop (Core 1).
- **Real-time VU meters**
  - Left/Right level meters for quick monitoring.
- **Tone controls**
  - Adjustable **Volume**, **Bass**, **Treble**.
  - Optional **Loudness** contour.
- **Speaker / Headphone mode**
  - Supports switching between speaker output (MONO) and headphones (STEREO) manually.
- **Screen Lock**
  - Short touch on the Upper Right corner switch to Screen Lock.
  - To unlock, touch the screen for about 4 seconds.

## Requirements

- **M5Stack TAB5**
- **microSD card** formatted and accessible by the device
- Your audio files placed in:
  - `SD:/Music`

## How to use

1. Copy audio files to `SD:/Music`.
2. Insert the SD card into the TAB5.
3. Flash the firmware.
4. Use the touch UI to:
   - Browse tracks
   - Start/stop playback
   - Change pages
   - Adjust volume and tone
   - Monitor VU meters

## Notes

- File and format compatibility depends on the underlying audio decoders available in the build.
- Very large libraries may take longer to scan on boot.

## License

MIT (unless noted otherwise in third-party components).
