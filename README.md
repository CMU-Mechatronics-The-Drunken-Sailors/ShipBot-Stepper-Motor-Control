# Stepper-Motor-Control
Firmware for [SKR board](https://www.biqu.equipment/products/bigtreetech-skr-mini-e3-v2-0-32-bit-control-board-integrated-tmc2209-uart-for-ender-3) to drive stepper motors, used to control the gantry/end-effector on our robot.

Once this code is flashed onto the SKR board, the board listens for G-code commands coming from the Jetson Nano in order to drive each motor to a specific position.

[G-code commands](https://marlinfw.org/meta/gcode/) are follows: **G1 X[#] Y[#] Z[#]**

X range is (0, 184)

X color coding: RED, GREEN, YELLOW, BLUE 

Y range is (0, 216)

Y color coding: BLUE, RED, GREEN, BLACK

Z range is (0, 70)

Z color coding: BLUE, BLACK, YELLOW, ORANGE

To home: **G28 [Axis]**

Factory reset: **M502**

All ranges are in millimeters. Color coding is looking from the right-side up, so that you can read "BTT SKR MINI".
