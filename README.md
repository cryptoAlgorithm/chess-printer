# Chess Printer

> A chess bot, but on steroids.

A completely custom-designed 3D printer control board with
an ESP32 MCU. Designed to control a CoreXY printer, but can
probably be adapted to any kinematic system.

## Notable Features

* 6 stepper drivers (labelled X, Y, E0, Z1, Z2 & Z3)
  - Designed for TMC2209 drivers
  - 1-wire Serial communication with all drivers supported
* ATX & screw terminal power input, `PS-ON` control
  - MCU can be powered from `5VSB` ATX power rail with jumper selection
* ESP32 MCU
* I2S stepper stream
  - 2x daisy-chained `75HC595` shift registers
* I2C LCD
* 1 hotend & 1 heatbed thermistor input
* 1 high power MOSFET bed heater & 1 heatbed output (for external relay/SSR)
* 1 controllable & 1 always-on fan output
