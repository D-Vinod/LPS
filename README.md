# Linear Power Supply (LPS)

**Circuit Diagram:**

![1](https://github.com/D-Vinod/LPS/assets/92619641/d1b682b6-4131-41ee-acfd-016b58deb3ff)

*Components:*
- BC109 x 2 Transistor
- BD139 Transistor
- BZX79-B/C4V7 Zener Diode
- 1k Ohm Potentiometer
- 220 Ohm 1/4W 5% resistor
- 10 Ohm 1/4W 5% resistor
- 1k Ohm 1/4W 5% resistor
- 1.2k Ohm 1/4W 5% resistor
- 100 Ohm 1/4W 5% resistor x 4

*Calculations:*
- Input Voltage range: 16V to 20V
- Output Voltage range: 8V to 14V
- Current Limit = 100mA

Maximum voltage difference = (20 – 8) V = 12V

Maximum power rating of T1 should be at least 0.1A x 12V = 1.2W

Chosen transistor for T1 - BD139 (In-built Heat sink) :

<img width="600" alt="2" src="https://github.com/D-Vinod/LPS/assets/92619641/06f7a6cd-81bc-42ca-9588-56d0cb8320ac">


Chosen Zener Voltage – 4.7 V (BZX79-B/C4V7)

<img width="600" alt="3" src="https://github.com/D-Vinod/LPS/assets/92619641/e56c6203-4330-4cce-9fc3-f29eecbd2147">


Calculation for Voltage regulaion,

<img width="600" alt="4" src="https://github.com/D-Vinod/LPS/assets/92619641/b9d1c0e1-0212-4762-a586-8c649b2af06d">

Calculation for Current regulaion,

VBE (ON) voltage of BC109 is nearly 0.77V. Therefore, to limit current at 100mA, a 7.7 Ohm resistance is needed. This resistance was achieved by a 10 Ohm resistor in the actual implementation.

*Results*
- Output Voltage Range – 8.4V – 14.4V
- Limiting Current – 100.0027A

<img width="600" alt="5" src="https://github.com/D-Vinod/LPS/assets/92619641/5fc3f82f-36e5-4df2-b740-f2c13a5d47b4">

