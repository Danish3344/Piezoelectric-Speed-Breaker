# Working Principle

When a vehicle passes over the proposed speed breaker, the top surface experiences mechanical loading. A mechanical transmission structure transfers controlled deformation to piezoelectric transducers.

The piezoelectric material produces an electrical output in response to mechanical stress. Because the raw output is not directly suitable for most electronic loads, it passes through a power-conditioning stage.

### Energy Flow

1. Vehicle applies mechanical force.
2. Mechanical structure distributes the force.
3. Piezoelectric elements undergo controlled deformation.
4. Electrical output is generated.
5. Rectifier converts the generated waveform into a usable DC form.
6. Protection and filtering reduce electrical stress and ripple.
7. Energy is accumulated in storage.
8. A regulator supplies the intended low-power load.
9. ESP32 monitors electrical parameters.

### Key Variables

Prototype testing should investigate:

- Applied force
- Piezo displacement
- Piezo element count
- Series/parallel configuration
- Open-circuit voltage
- Loaded voltage
- Load current
- Energy harvested per compression
- Energy harvested per vehicle passage
- Storage charging rate
- Mechanical cycle count
- Temperature and environmental conditions

No numerical performance result is assumed until experimental measurements are available.
