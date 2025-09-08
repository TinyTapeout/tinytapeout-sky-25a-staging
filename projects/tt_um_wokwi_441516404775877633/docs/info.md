<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

A thermometer code at the input IN<7:0> is displayed on the 7-segment display as if the display is filling up like a vessel, startin with 'DP' ending at segment 'a'.
The inputs are syncronized to the clock using two D-FFs.

- IN<7> ... a
- IN<6> ... b
- IN<5> ... f
- IN<4> ... g
- IN<3> ... c
- IN<2> ... e
- IN<1> ... d 
- IN<0> ... DP

## How to test

Apply test codes e.g. by using a 8-bit input switch to generate a thermometer code 
- 0b00000000; SEGS: -
- 0b00000001; SEGS: DP
- 0b00000011; SEGS: DP, d
- .
- .
- .
- 0b00111111; SEGS: DP, d, e, c, g, f
- 0b01111111; SEGS: DP, d, e, c, g, f, b
- 0b11111111; SEGS: DP, d, e, c, g, f, b, a

## External hardware

- 7 Segment display
  - OUT<0>: SEG-a
  - OUT<1>: SEG-b
  - OUT<2>: SEG-c
  - OUT<3>: SEG-d
  - OUT<4>: SEG-e
  - OUT<5>: SEG-f
  - OUT<6>: SEG-g
  - OUT<7>: SEG-DP
  - COM1: GND
