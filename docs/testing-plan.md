# Testing Plan

## Phase 1 — Individual Transducer

Measure:

- Open-circuit voltage
- Loaded voltage
- Current through defined loads
- Response to controlled mechanical compression

## Phase 2 — Array

Compare series, parallel, and mixed configurations using the same controlled mechanical input.

Record:

- Peak voltage
- RMS voltage where applicable
- Load current
- Energy per compression
- Rectifier losses

## Phase 3 — Mechanical Prototype

Use controlled loads before vehicle testing.

Verify:

- Maximum displacement
- Force distribution
- Return mechanism
- Mechanical stops
- Piezo protection
- Structural stability

## Phase 4 — Vehicle Testing

Only after controlled-load validation:

1. Test with low-speed controlled vehicle passes.
2. Record electrical measurements.
3. Repeat multiple passes.
4. Compare results under different vehicle loads/speeds.
5. Inspect mechanical components after each test series.

## Measurements

For a measured voltage-current operating point:

```
P = V × I
```

Accumulated energy can be estimated by integrating power over time:

```
E = ∫ P(t) dt
```

For discrete sampled data, numerical integration can be used.

## Safety

The prototype must not compromise normal vehicle passage, road safety, structural integrity, or electrical safety. Vehicle testing should be conducted only in a controlled and authorized environment.
