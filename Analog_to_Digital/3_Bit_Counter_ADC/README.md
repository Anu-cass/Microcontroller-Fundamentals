A 3-bit counter-type ADC

Construction: It uses a Comparator, a 3-bit Digital-to-Analog Converter (DAC), a 3-bit Binary Counter, a Clock, and an AND gate as control logic.

Working:

Reset: The counter starts at 000. The DAC outputs 0V.

Count & Compare: The counter starts incrementing, and the DAC converts each count into a slightly higher analog voltage (a "ramp").

Stop: The Comparator continuously compares this increasing DAC voltage to the Analog Input Voltage (V in​).

Digital Output: When the DAC voltage equals or just exceeds V in​, the comparator tells the AND gate to stop the counter. The digital value currently in the counter is then the ADC's 3-bit output.
