# Arduino Communication: Transmitter and Receiver Project

This project demonstrates serial communication between two Arduino UNO boards (ARD1 and ARD2). It uses a transmitter module (push button interface) and a receiver module (relay and lamp control system) to turn on/off electrical loads.

---

##  Components Used

- 2 × Arduino UNO
- 2 × Push Buttons
- 2 × Resistors (330Ω)
- 2 × NPN Transistors (BC547)
- 2 × Relays (12V)
- 2 × Diodes (1N4007)
- 2 × Lamps (12V)
- Jumper Wires
- External 12V Power Supply
- Breadboard or PCB (optional)

---

##  Working Principle

- **ARD1 (Transmitter):**
  - Reads button inputs.
  - Sends a signal via Serial Tx to ARD2 when buttons are pressed.

- **ARD2 (Receiver):**
  - Receives serial data.
  - Depending on input, it activates transistors and relays.
  - The relays turn on/off the connected lamps.

---

##  Connections

### Transmitter (ARD1):
| Component | Arduino Pin |
|----------|-------------|
| Button 1 | D2          |
| Button 2 | D3          |
| Tx       | Connect to Rx of ARD2 |

### Receiver (ARD2):
| Component     | Arduino Pin |
|--------------|-------------|
| Relay 1 Input| D2          |
| Relay 2 Input| D3          |
| Rx           | Connect to Tx of ARD1 |

---

##  Code Files

- `Transmitter.ino` – Arduino sketch for button detection and serial transmission.
- `Receiver.ino` – Arduino sketch for receiving data and activating relay/lamp.

---

##  Communication Setup

- Serial Communication: 9600 baud rate
- Connection: Tx (ARD1) → Rx (ARD2)

---

##  Preview

Proteus simulation snapshot included.

---

## 💡 Applications

- Remote load switching
- Home automation basics
- Learning serial communication
- Wireless controls (with RF/HC-12 upgrade)

---



