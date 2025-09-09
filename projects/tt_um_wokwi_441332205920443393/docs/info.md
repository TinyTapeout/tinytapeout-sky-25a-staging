<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

A 16 bit counter is implemented, but only the last 8 bits are used as outputs. This way, the clock frequency of 10 kHz is reduced to a counting frequency of around 2,5 Hz. When reset is pressed, the value of the counter is set to 0. When an overflow occurs, the counter starts again at 0.

## How to test

Power on the circuit and watch the counter increase. The LED's connected to OUT0 - OUT7 show a binary representation of the counter value.

## External hardware

8 LED's are used at the pins OUT0 - OUT7 to show the current value of the counter.
