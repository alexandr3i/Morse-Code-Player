# Morse Code Player (Arduino)

This practical project displays characters received over the **Serial Monitor** as **Morse code** on a screen and, at the same time, plays the corresponding beeps through a **buzzer**.

Goal: communicate messages in **Morse code** using an Arduino-based device.

---

## Repository contents
- `MorseCode-Arduino.ino` — Arduino sketch (main program)
- `Morse Code Player Docuementation.pdf` — project documentation (report)

---

## Hardware (typical setup)
- Arduino board (Uno / Nano / similar)
- Display (as used in your setup; see the PDF for the exact model)
- Active or passive buzzer (connected to a digital pin)
- Wires / breadboard

Note: the exact pins and display library depend on your build; follow the wiring/pin map described in the PDF documentation.

---

## How to run

1. Download the repository (Code → Download ZIP) or clone it.
2. Open `MorseCode-Arduino.ino` in **Arduino IDE**.
3. Install any required display libraries (if the sketch uses one). If you get a “missing library” error on compile, install that library from Arduino IDE → Library Manager.
4. Select your board and port in Arduino IDE (Tools → Board / Port).
5. Upload the sketch to the Arduino.

---

## How to use
1. Open Arduino IDE → Tools → **Serial Monitor**.
2. Set the correct bit rate (must match the value in the sketch; common values are 9600 or 115200).
3. Type a character or short text message in the Serial Monitor input field and send it.
4. The device will:
   - show the Morse pattern on the display (dots/dashes or equivalent visual representation)
   - play the Morse sound pattern on the buzzer

---

## Notes / limitations
- Morse support depends on what characters are implemented in the sketch (letters, digits, and/or symbols).
- Timing (dot/dash speed) is controlled by delays/constants in the code.
- This is a hardware-dependent project; it requires an Arduino + display + buzzer to demonstrate.

---

## License
Educational use only. This repository is intended for learning, demonstration, and portfolio/documentation purposes.
