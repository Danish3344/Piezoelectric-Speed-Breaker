# ESP32 Monitoring Firmware

The ESP32 firmware will be developed to monitor the electrical subsystem after the hardware design is validated.

## Planned Measurements

- Storage voltage
- Load current
- Estimated instantaneous power
- Accumulated harvested energy
- System state
- Optional temperature

## Planned Data Flow

```
Voltage Sensor ─┐
                ├──> ESP32 ───> Serial Monitor
Current Sensor ─┘       |
                        └──────> Optional OLED / Dashboard
```

## Firmware Status

**Not yet implemented.**

The firmware will only use sensor scaling values verified against real hardware measurements. No fabricated sensor readings will be included in the repository.
