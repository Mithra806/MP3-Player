# MP3 Player — KiCad Hardware Project

A rechargeable MP3 player I designed from scratch in KiCad. It's got buttons
for playback control and a small screen that shows what track is playing.

## What it does
- Charges over USB
- Plays MP3s off a microSD card, using a DFPlayer Mini module
- Headphone output via a 3.5mm jack
- Two buttons for next/previous track and volume
- An OLED screen shows the current track, driven by an Arduino Nano reading
  data from the DFPlayer Mini (not programmed yet)
- A power switch to turn the whole thing on/off

## Bill of Materials
| Ref | Component | Value/Notes | Qty | Link |
|-----|-----------|-------------|-----|------|
| BT1 | 18650 Li-ion Battery | 3.7V rechargeable cell | 1 | [Link](#) |
| SW1 | Slide/Toggle Switch | Power switch, SPST | 1 | [Link](#) |
| SW2 | Pushbutton | Next track (wired to DFPlayer IO1) | 1 | [Link](#) |
| SW3 | Pushbutton | Previous track (wired to DFPlayer IO2) | 1 | [Link](#) |
| SW4 | Pushbutton | Pause/Unpause (wired to Arduino D2) | 1 | [Link](#) |
| U1 | TP4056-42-ESOP8 | Li-ion charger IC | 1 | [Link](#) |
| U2 | DFPlayer Mini | MP3 playback module | 1 | [Link](#) |
| U3 | OLED Display | ER-OLEDM0.91-1x-I2C (SSD1306-based) | 1 | [Link](#) |
| A1 | Arduino Nano v3.x | Microcontroller | 1 | [Link](#) |
| J1 | 3.5mm Audio Jack | Mono, 5-pin | 1 | [Link](#) |
| J2 | USB Micro-B Connector | Charging input | 1 | [Link](#) |
| R1 | Resistor | 2kΩ (sets TP4056 charge current) | 1 | [Link](#) |
| — | microSD Card | Stores audio files for DFPlayer | 1 | [Link](#) |
| — | Headphones/Speaker | Audio output | 1 | [Link](#) |

## Schematic

<img width="516" height="387" alt="image" src="https://github.com/user-attachments/assets/479fbc55-b09f-455f-aff5-b23b7ed8d56c" />

## PCB Layout

<img width="600" alt="PCB Layout" src="https://github.com/user-attachments/assets/3e60f064-c293-4bbd-bc82-38581a1b8835" />

## 3D Render

<img width="600" alt="3D Render" src="https://github.com/user-attachments/assets/16434667-0b96-41c6-bb2b-35317c6dd804" />
