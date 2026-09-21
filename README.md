# rtos-supervision-node

Real-time supervision and control node built on FreeRTOS (STM32L476RG).

The goal is not just a working system: the timing behaviour of every task is
computed analytically first, then verified against measurements taken on the
hardware.

## Hardware

- NUCLEO-L476RG (Cortex-M4 @ 80 MHz)
- Logic analyser for timing measurements
- I2C sensor, potentiometer

## Toolchain

STM32CubeIDE / CubeMX / HAL / FreeRTOS

## Results

_To be filled as milestones complete._

| Metric | Predicted | Measured |
|---|---|---|
| Context switch time | — | — |
| Task jitter | — | — |
| CPU load | — | — |

## Milestones

- [x] M0 — Repository and project skeleton
- [ ] M1 — Two tasks, measurement baseline
- [ ] M2 — Real-time acquisition (TIM + ADC + DMA)
- [ ] M3 — Slow sensor and shared state
- [ ] M4 — State machine and fault handling
- [ ] M5 — UART shell
- [ ] M6 — Observability and measurement campaign
- [ ] M7 — Hardening and documentation

## Documentation

- [Architecture](docs/architecture.md)
- [Timing analysis](docs/timing-analysis.md)
- [Measurements](docs/measurements.md)
- [Design log](docs/design-log.md)