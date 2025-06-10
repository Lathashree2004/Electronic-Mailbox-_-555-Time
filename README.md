# 📬 Electronic Mailbox Using 555 Timer

This project is a simple **mail detection system** using a 555 Timer IC and LDR. It visually alerts the user using LEDs when a letter or envelope is inserted into the mailbox.

---

## 🛠️ Features

- Detects physical mail using a Light Dependent Resistor (LDR).
- Uses 555 Timer IC in comparator mode.
- Visual alert with LEDs:  
  - Green LED (Light falling on LDR)  
  - Red LED (Mail inserted – light blocked)
- Adjustable sensitivity using a potentiometer.
- Battery powered – ideal for low-power setups.

---



## 📋 Working Principle

- A **green LED** constantly illuminates the LDR.
- When light is falling on the LDR (no mail), its resistance is low → **Output = Yellow colour LED ON (safe)**.
- When light is blocked by an object (mail), LDR resistance increases → **Output = RED LED ON (mail received)**.
- A **10kΩ potentiometer** sets a reference voltage to compare against the LDR voltage via the 555 Timer.

---

## 🔧 Components Used

| Component         | Quantity |
|------------------|----------|
| 555 Timer IC      | 1        |
| Light Dependent Resistor (LDR) | 1 |
| Potentiometer (10kΩ) | 1      |
| LED – Green       | 1        |
| LED – Red         | 1        |
| Resistors (470Ω, 10kΩ) | 3+ (may vary) |
| 9V Battery        | 1        |
| Breadboard + Jumper Wires | - |

---

## 📈 Conditions Table

| Condition         | LDR   | Voltage | Compared to Pot | Output     |
|------------------|-------|---------|-----------------|------------|
| Bright (light on LDR) | Low   | Low     | V_LDR < V_ref   | LED ON     |
| Dark (mail blocks light) | High  | High    | V_LDR > V_ref   | LED OFF / Alert |

---

## 💡 Improvements

- Replace red LED with a **buzzer** for audio alert.
- Enclose the setup inside a weatherproof mailbox unit.
- Add Arduino for smart notifications via Wi-Fi.

---

## 📚 License

This project is open-source and free to use for educational and non-commercial purposes.

---

