> A hardware-based Digital Clock built using discrete ICs without a microcontroller.

---

## 📌 Overview
A digital clock designed entirely using digital electronics. The project demonstrates the fundamentals of counters, clock division, sequential logic, and seven-segment display interfacing without relying on programmable devices such as Arduino or ESP32.

The clock displays time in **24-hour format (HH:MM:SS)** and includes **AM/PM indication** using LEDs.

This project is intended for educational purposes to strengthen understanding of Digital Electronics and Hardware Design.

---

## ✨ Features

- 24-Hour Time Format
- Hours, Minutes, and Seconds Display
- AM / PM LED Indicator
- CMOS Logic Design
- Breadboard Prototype
- Expandable to PCB Design
- No Microcontroller Required

---

## 🛠 Hardware Used

### ICs

- CD4026 Decade Counter with 7-Segment Driver
- NE555 Timer
- Logic Gates

### Displays

- Common Cathode 7-Segment Displays

### Passive Components

- Resistors
- Capacitors
- Crystal / RC Timing Components
- Push Buttons
- LEDs

### Power

- 5V Regulated Supply

---

## ⚙️ Working Principle

1. A clock pulse is generated using an oscillator.
2. The pulse is converted into a precise 1 Hz signal.
3. CD4026 ICs count the pulses.
4. Each CD4026 directly drives a seven-segment display.
5. Counter carry outputs cascade into the next digit.
6. Logic resets counters at appropriate values:
   - Seconds: **59 → 00**
   - Minutes: **59 → 00**
   - Hours: **12 → 01**
7. The AM/PM indicator toggles every 12 hours.

---

## 📂 Repository Structure

```text
Digital_clock/
│
├── docs/
│   ├── BlockDiagram.png
│   ├── CircuitDiagram.pdf
│   ├── BreadboardLayout.png
│   └── ProjectReport.pdf
│
├── kicad/
│   ├── Schematic/
│
│
├── images/
│   ├── Prototype.jpg
│   ├── FinalClock.jpg
│   └── Wiring.jpg
│
├── README.md
└── LICENSE
```

---

## 🚀 Project Status

Current Stage:

- [x] Project Planning
- [x] Component Selection
- [ ] Schematic Design
- [ ] Breadboard Prototype
- [ ] Functional Testing
- [ ] PCB Design
- [ ] Final Documentation

---

## 📚 Concepts Used

- Digital Electronics
- Sequential Logic
- Decade Counters
- Frequency Division
- Seven-Segment Displays
- Clock Generation
- Reset Logic
- Cascaded Counters

---

## 🎯 Future Improvements

- Alarm Function
- Stopwatch Mode
- Date Display

--

---

## 📜 License

This project is released for educational and learning purposes.
