# Arduino Distance Calculator (HC-SR04)

Simple beginner-friendly project to measure distance using an Arduino Uno and the HC-SR04 ultrasonic sensor.

## What’s included
- `DistanceCalculator_Serial.ino` — Complete Arduino sketch (Serial output).
- `wiring.txt` — Text blueprint / wiring diagram.
- `README.md` — This file.
- `LICENSE` — MIT License.

## Parts required
- Arduino Uno (or compatible)
- HC-SR04 ultrasonic sensor
- Jumper wires (Male-Female)
- USB A-to-B cable
- Ruler (for demo/calibration)

## Wiring (4 connections)
| HC-SR04 Pin | Arduino Pin |
| ----------- | ----------- |
| VCC         | 5V          |
| GND         | GND         |
| TRIG        | D9          |
| ECHO        | D10         |

See `wiring.txt` for a simple ASCII blueprint.

## How to use
1. Connect the HC-SR04 to the Arduino using the wiring above.
2. Open the Arduino IDE, create a new sketch, paste the contents of `Distance_Calculator.ino`.
3. Select the correct board and COM/port.
4. Verify (compile) and Upload.
5. Open the Serial Monitor (Tools → Serial Monitor) and set baud to **9600**.
6. Move an object in front of the sensor and watch the distance readings.

## Notes & Troubleshooting
- Typical HC-SR04 working range: ~2 cm to ~400 cm.
- If you see `Out of range` frequently, check wiring and ensure the target is reflective and perpendicular.
- If readings are noisy, shorten wires and avoid obstacles in sensor path.
- If `pulseIn` returns 0 often, try increasing timeout or check power connections.

## License
This project is released under the MIT License — see `LICENSE`.
