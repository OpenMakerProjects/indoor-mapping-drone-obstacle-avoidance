# Wiring guide

This is a low-voltage prototype wiring plan for **Indoor Mapping Drone Obstacle Avoidance**. Confirm every module's datasheet because breakout-board pinouts vary.

| Component | Suggested pin | Role | Check |
| --- | --- | --- | --- |
| optical flow sensor | A0 | Analog input | Confirm the module voltage and pinout before power-up. |
| battery monitor | 5 | Digital I/O | Confirm the module voltage and pinout before power-up. |
| IMU | 6 | Digital I/O | Confirm the module voltage and pinout before power-up. |
| Status output | LED_BUILTIN | Output | Use a resistor when an external LED is fitted. |

## Power

- Use a regulated supply sized for the selected modules.
- Join grounds unless an interface is explicitly isolated.
- Do not connect mains voltage directly to a development board.
- Add a fuse, emergency stop, and certified isolation where a real actuator can create risk.
