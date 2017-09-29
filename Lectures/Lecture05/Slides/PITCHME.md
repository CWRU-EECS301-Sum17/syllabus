---

# Lab 4 Review

Note:
Lab 4 Questions, Issues, Feedback?

---

## Serial Devices

* UART (RS-232)
* PS/2 (Keyboard)
* Telegraph

---

**Universal Asynchronous Receiver-Transmitter**

* Signaling protocol
* Widely used for RS-232, RS-422, RS-485 Bus Standards
* Supported by most embedded systems (for terminal)
* Basic Error Detection (Optional)
* Configurable Data Payload (usually 7/8/9-bits)

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture05/Slides/images/UART_Data_Frame.png&size=95% auto

Note:
Typical Data Frame: 8 Data Bits, No Parity Bit, 1 Stop Bit

---

### Asynchronous Transmit

* Data transmitted without accompanying Clock
* Transmitter and Receiver have independent Clocks
* No phase relationship between Transmitter and Receiver
* Receiver re-aligns to Transmitter on Start Bit
* Transmission speed called Baud Rate

---

## PS/2 Keyboard Bus

* Introduced by IBM in 1987 PS/2 Computer
* Mostly phased out by USB (security/compatibility uses)
* Synchronous Clock and Data Signals
* Bi-directional Data

Note:
PS/2 used on systems with USB disabled for security.
Better BIOS support than USB

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture05/Slides/images/PS2_Keyboard_Data_Frame.png&size=95% auto

---

# Lab 5 Overview

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture05/Slides/images/Lab5_DevBoardLayout.jpg&size=90% auto

---
