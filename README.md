# Piezoelectric Speed Breaker

A prototype concept for harvesting mechanical energy from vehicles passing over a speed breaker using piezoelectric transducers and converting it into usable electrical energy.

> **Project status:** Concept / Prototype Development  
> This repository documents the engineering design, calculations, firmware plan, testing methodology, and future prototype work. No physical performance results are claimed until measured experimentally.

## Objective

To design a speed-breaker-based energy harvesting system that converts vehicle-induced mechanical pressure into electrical energy through piezoelectric transducers, stores the harvested energy, and provides basic monitoring of voltage, current, energy, and system status.

## Proposed System

Vehicle load  
→ Mechanical compression mechanism  
→ Piezoelectric transducer array  
→ Rectification  
→ Voltage regulation / protection  
→ Energy storage  
→ DC-DC regulation  
→ ESP32 monitoring

## Planned Features

- Modular piezoelectric transducer array
- Mechanical force-transfer structure
- AC-to-DC rectification
- Energy storage using a suitable rechargeable storage element
- Voltage/current monitoring
- ESP32-based data acquisition
- Optional OLED/local dashboard
- Experimental energy-per-vehicle characterization
- Safety-focused mechanical enclosure

## Repository Structure

```
.
├── docs/
│   ├── system-architecture.md
│   ├── working-principle.md
│   ├── hardware-design.md
│   ├── energy-calculations.md
│   ├── testing-plan.md
│   └── future-improvements.md
├── hardware/
│   ├── bom.md
│   ├── circuit/
│   └── mechanical-design/
├── firmware/
│   └── esp32/
├── simulations/
├── tests/
└── README.md
```

## Important Engineering Note

Individual piezoelectric elements can produce relatively high open-circuit voltage but limited current. Practical system performance therefore depends on the transducer type, mechanical coupling, array configuration, rectifier losses, storage method, vehicle load, displacement, and operating frequency. All output-power claims will be based on measurements after the prototype is built.

## Development Roadmap

- [x] Define project objective
- [x] Define system architecture
- [x] Establish repository structure
- [ ] Select piezoelectric transducer and mechanical arrangement
- [ ] Complete electrical design
- [ ] Complete mechanical design
- [ ] Implement ESP32 monitoring firmware
- [ ] Build laboratory prototype
- [ ] Perform controlled-load testing
- [ ] Perform vehicle-load testing
- [ ] Record measured energy output
- [ ] Analyze efficiency and durability
- [ ] Document final prototype

## Applications

The concept can be investigated for low-power applications such as indicator lighting, sensing, telemetry, or energy-aware roadside systems where harvested energy is sufficient for the intended load.

## Author

**Danish**  
B.E. Electronics and Communication Engineering

## License

MIT License
