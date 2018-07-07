---
title: "National Undergraduate Electronics Design Contest"
collection: teaching
type: "Design of a Simple Frequency Meter"
permalink: /teaching/2014-spring-teaching-1
venue: " "
date: 2015-07-15
location: "City, Country"
---

In July 2015, together with two other classmates, I participated in the National Undergraduate Electronic Design Competition. One classmate was responsible for software programming, the other finished the game report and helped us debugging. I was responsible for designing hardware circuit making and debugging.Our team chose the F question, designing and building the simple digital frequency within the relatively short contest time of 3 days and 4 nights, and the scores of the F question are as follows:

Design and build a digital frequency meter with a gate time of 1s
* the requirements
* 1 . basic requirements
* (1) Frequency and period measurement function
    * a. The measured signal is a sine wave with a frequency range of 1 Hz to 10 MHz;
    * b. The measured signal rms voltage range is 50mV ~ 1V;
    * c. The absolute value of the measured relative error is not more than 0.0001.
* (2) Time interval measurement function
    * a. The measured signal is a square wave with a frequency range of 100 Hz to 1 MHz;
    * b. The peak-to-peak value of the measured signal peak-to-peak value ranges from 50mV to 1V;
    * c. The measured time interval ranges from 0.1 μs to 100 ms;
    * d. The absolute value of the measured relative error is not more than 0.01.
* (3) The measurement data refresh time is no more than 2s, the measurement result is stable, and the unit can be automatically displayed.
* 2 . Improve part
* (1) The frequency range and period measurement of the sinusoidal signal frequency range is 1Hz ~ 100MHz, other requirements are the same as basic requirement (1) and (3).
* (2) The minimum rms voltage (voltage RMS) of the sinusoidal signal measured during frequency and period measurement is 10mV, other requirements are the same as basic requirements (1) and (3).
* (3) Increase the pulse signal duty cycle Duty cycle measurement function, requires:
    * a. The measured signal is a rectangular wave Rectangular wave with a frequency range of 1 Hz to 5 MHz;
    * b. The peak-to-peak voltage of the measured signal ranges from 50mV to 1V;
    * c. The duty cycle of the pulse signal to be measured ranges from 10% to 90%;
    * d. The resolution displayed is 0.1%, and the absolute value of the measured relative error is not more than 0.01.
* (4) Others (for example, further reducing the amplitude of the signal voltage to be measured, etc.).

In the end, our work completed the basic requirements of this question, but the measurement below 10Hz is unstable. As for improve requirements, we achieved the max measuring frenqucy 80MHz, the minimum RMS voltage 15mV finally, limited by the amplifier's Gain Bandwidth Product (GBW), and the a,b,c requirement of duty cycle measurement was also achieved. 

But in the actual examination process, it was unfortunate that the circuit problem occured, and finally the measurement feil in over 10Mhz and below 50mv. The main reason was the relay switch I used, which should have been only controlled by the FPGA controller instead of the manual switch. Because there is a requirement,no manual operation for the control signal. In addition, lack of stability of the circuit is another reason for the malfunction in the field.

We won the third prize finally.
