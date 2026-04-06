# SunKeyer v1.0A

**Voice Keyer for SunSDR Transceivers via TCI**

Designed by Chris Lawton, M7JEX. Somerset, UK.

---

## Overview

SunKeyer is a Windows voice keyer application designed specifically for SunSDR transceivers running ExpertSDR2 or ExpertSDR3. It connects directly to the radio via the **TCI (Transceiver Control Interface)** protocol over WebSocket — no VAC, no virtual audio cable, no sound card routing required. Audio is streamed directly into the radio.

---

## Screenshots

### Light Mode
![Light Mode](SCREENSHOTS/LIGHT%20MODE.jpg)

### Dark Mode
![Dark Mode](SCREENSHOTS/DARK%20MODE.jpg)

### Main Menu
![Main Menu](SCREENSHOTS/MAIN%20MENU.jpg)

### Recording a Macro
![Recording Button](SCREENSHOTS/RECORDING%20BUTTON.jpg)

---

## Features

- **6 macro buttons** — Each independently named and recorded
- **Direct TCI audio streaming** — Audio goes straight into ExpertSDR, no VAC needed
- **Auto PTT** — Keys the radio automatically before playback, drops after
- **Repeat mode** — Automatic CQ repeat with user-selectable interval and countdown timer
- **VU meter** — Gradient bar with SAFE / WARN / CLIP zones, peak hold, dBFS readout
- **VU Meter Always Active** — option to monitor mic level continuously
- **Record Level slider** — controls recording gain independently
- **Light and Dark mode** — switchable from the File menu, remembers your preference
- **Display on top** — optional always-on-top window mode
- **TX elapsed timer** — shows how long you have been transmitting
- **Settings persistence** — all button names, recordings and settings saved between sessions

---

## Requirements

- Windows 7 TO 11 (64-bit only)
- ExpertSDR2 or ExpertSDR3 with TCI enabled

---

## Installation

1. Download `SunKeyer_Setup_v1.0A.exe` from the releases page
2. Run the installer and follow the on-screen instructions
3. Launch SunKeyer from the desktop shortcut or Start Menu

No additional software required. SunKeyer is fully standalone.

---

## Setting Up TCI in ExpertSDR

1. Open ExpertSDR2 or ExpertSDR3
2. Go to **Options → TCI**
3. Make sure TCI is enabled
4. Note the port number:
   - ExpertSDR2 default: **40001**
   - ExpertSDR3 default: **50001**
5. In SunKeyer, enter `localhost` as the host and your port number
6. Click **Connect** — the button will turn green when connected

---

## Recording a Macro

1. Make sure your microphone is selected under **File → Select Microphone**
2. Press and hold the **REC** button on any macro slot
3. Hold for 3 seconds — a countdown ring fills around the button
4. When the ring completes the recording starts. The button flashes red to indicate macro is now being recorded
5. Speak your message
6. Press the button again to stop recording
7. Press **SAVE** to save the recording to disk
8. The button now shows **▶ TX** and is ready to transmit

---

## Transmitting

1. Click **▶ TX** on any recorded macro
2. SunKeyer automatically keys the radio via TCI, streams the audio, then drops PTT
3. To stop mid-transmission press **■ STOP TX** or the **ABORT** button

---

## Repeat Mode

1. Set your repeat interval in seconds
2. Toggle **Repeat ON**
3. Press **▶ TX** on your chosen macro
4. SunKeyer will automatically repeat the transmission at your chosen interval
5. A countdown shows time to next TX
6. Press **ABORT** to stop repeating at any time

---

## Deleting A Macro

1 Right click on the macro name and confirm deletion

---

## Renaming A Macro

1 left double click on the macro name, then enter the amended name for the macro

---



## Licence

SunKeyer is provided free of charge for personal, non-commercial use by licensed amateur radio operators and the wider amateur radio community.

Selling for profit or modifying this software is strictly prohibited.

See [LICENSE.txt](LICENSE.txt) for full terms.

---

## About

Designed by **Chris Lawton, M7JEX**  
Somerset, United Kingdom.  

73 M7JEX
