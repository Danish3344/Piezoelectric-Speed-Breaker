# System Architecture

## High-Level Architecture

```
Vehicle Load
     |
     v
Mechanical Top Plate
     |
     v
Force Distribution / Compression Mechanism
     |
     v
Piezoelectric Transducer Array
     |
     v
Rectifier + Protection
     |
     +------> Voltage / Current Sensing
     |
     v
Energy Storage
     |
     v
DC-DC Regulation
     |
     +------> Low-Power Load
     |
     v
ESP32 Monitoring
     |
     +------> OLED / Serial / Future Dashboard
```

## Functional Blocks

### 1. Mechanical Layer
Transfers a controlled portion of vehicle-induced force to the piezoelectric elements while limiting excessive displacement and protecting the transducers.

### 2. Piezoelectric Conversion Layer
Piezoelectric elements generate an electrical response when mechanically stressed. Multiple elements can be combined into an array depending on the selected electrical configuration.

### 3. Power Conditioning
The raw piezoelectric output is conditioned using rectification, protection, filtering, and appropriate regulation before storage.

### 4. Energy Storage
The conditioned energy is accumulated in a storage element selected according to voltage, current, cycle life, safety, and expected harvested energy.

### 5. Monitoring
An ESP32 can measure system parameters such as storage voltage, load current, estimated power, accumulated energy, and operating state.

## Design Principle

The system should prioritize mechanical reliability and controlled force transfer rather than simply maximizing the instantaneous voltage produced by an unloaded piezoelectric element.
