# CAN·Lab — Interactive Controller Area Network

An interactive learning site for the CAN protocol (real-time embedded systems course).

**Open it:** see the GitHub Pages link in this repository's About section.

## Slides
The lecture deck is at `/slides/`: a six-act story (“The Night the Brakes Had to Talk”) with live 3D models. The earlier design is at `/slides/classic/`. Use ← → to move, N for speaker notes, F for fullscreen and S to toggle the synthesized rain, thunder and atmosphere.

The five story clips in `slides/media/` are 3D renders (three.js, rendered frame by frame and encoded with ffmpeg); the characters and scenario are fictional.

## What's inside
- 3D CAN bus (three.js): click an ECU to transmit, or start all of them at once to watch arbitration
- Physical layer scope: CAN_H / CAN_L, differential voltage, common-mode noise
- Frame builder with live CRC-15 and bit stuffing
- Step-by-step bitwise arbitration lab
- Error counters and the fault-confinement state machine (error-active / error-passive / bus-off)
- Bit-timing calculator
- Worst-case response-time analysis (Davis et al., 2007), including their counterexample
- Classical CAN vs CAN FD vs CAN XL

The whole site is one self-contained `index.html`. It needs an internet connection for three.js and the fonts.

## References
1. Robert Bosch GmbH (1991). CAN Specification Version 2.0, Parts A & B.
2. ISO 11898-1:2015 / ISO 11898-1:2024; ISO 11898-2.
3. Tindell, Burns, Wellings (1994). Calculating CAN message response times. IFAC DCCS'94.
4. Davis, Burns, Bril, Lukkien (2007). CAN schedulability analysis: refuted, revisited and revised. *Real-Time Systems* 35(3):239–272. doi:10.1007/s11241-007-9012-7
5. Hartwich (2012). CAN with Flexible Data-Rate. iCC 2012.
6. CAN in Automation (CiA): CAN HS transmission, CAN XL.
