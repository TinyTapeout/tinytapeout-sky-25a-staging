<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

The circuit compares two 4-bit binary numbers, A and B, using only basic logic gates such as XOR, AND, OR and NOT. The values of A and B are set through the DIP switch, with inputs IN0 to IN3 representing A and inputs IN4 to IN7 representing B. The comparison starts with the most significant bit, where the logic checks whether a bit of A is higher than the corresponding bit of B. If the bits are equal, the comparison continues with the next lower bit until a difference is found. If at any point A has a higher bit than B, the circuit decides that A is greater than B. The output of this logic is connected to the 7-segment display, which shows the result directly: a “1” appears when A is greater than B, while a “0” is displayed when A is equal to or smaller than B. In this way, the project demonstrates how a binary magnitude comparator can be built entirely from simple logic gates.

## How to test

To test the circuit, start by setting different binary values for A and B using the DIP switch. The first four inputs (IN0 to IN3) represent the 4-bit number A, while the next four inputs (IN4 to IN7) represent the 4-bit number B. After selecting the values, the comparator logic evaluates them automatically. The 7-segment display then shows the result of the comparison: if A is greater than B, it lights up with a “1”, otherwise it shows “0”. By trying different switch combinations, you can verify that the display always updates correctly according to the relative size of the two numbers.

## External hardware

This project uses a DIP switch to provide the binary inputs A and B and a 7-segment display to show the comparison result.
