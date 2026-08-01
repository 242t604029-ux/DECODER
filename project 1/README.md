# 3-to-8 Decoder using Verilog HDL

## Overview

This project implements a **3-to-8 Decoder** in Verilog HDL. A decoder converts a binary input into one active output line while all remaining outputs stay inactive.

---

## Features

- Verilog HDL implementation
- Enable input
- One-hot output
- Complete testbench
- Simulation ready
- FPGA compatible

---

## Truth Table

| Enable | A2 A1 A0 | Output |
|---------|----------|--------|
|0|XXX|00000000|
|1|000|00000001|
|1|001|00000010|
|1|010|00000100|
|1|011|00001000|
|1|100|00010000|
|1|101|00100000|
|1|110|01000000|
|1|111|10000000|

---

## Folder Structure

```
Decoder-3x8-Verilog/
├── src/
├── testbench/
├── simulation/
└── docs/
```

---

## Simulation

### Using Icarus Verilog

```bash
iverilog -o decoder_sim src/decoder_3x8.v testbench/decoder_3x8_tb.v
vvp decoder_sim
```

### Using GTKWave

```bash
iverilog -o decoder_sim src/decoder_3x8.v testbench/decoder_3x8_tb.v
vvp decoder_sim
gtkwave decoder.vcd
```

### Using ModelSim

```text
vlib work
vlog src/decoder_3x8.v
vlog testbench/decoder_3x8_tb.v
vsim decoder_3x8_tb
run -all
```

---

## Applications

- Memory Address Decoding
- Instruction Decoding
- Digital Logic Design
- FPGA Projects
- Embedded Systems

---

## Author

Your Name