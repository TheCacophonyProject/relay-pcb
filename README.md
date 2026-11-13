# relay-pcb

A relay board that lets a thermal camera switch another device on and off. The relay contacts are
isolated from the camera.

## Wiring

### Power and control (one of these)

- **Camera plug (J1):** connect the M16 cable from the camera's output plug. The camera powers the
  board and switches the relay.
- **Screw terminal (J3):**

  | Terminal | Connect to |
  | --- | --- |
  | 12V | 12V supply (+) |
  | GND | supply ground (-) |
  | SIG | control signal: 3.3V to 12V = relay on, 0V or unconnected = relay off |

### Switched device (J2)

Wire the device you want to switch to the J2 screw terminal:

| Terminal | Use |
| --- | --- |
| COM | common, always used |
| NO | normally open: connected to COM only when the relay is on |
| NC | normally closed: connected to COM only when the relay is off |

For most uses, wire the device's supply through COM and NO, so the device only gets power while the
relay is on.

The red LED lights while the relay is on.

## License

CERN Open Hardware Licence Version 2 - Weakly Reciprocal (see [LICENSE](LICENSE)).
