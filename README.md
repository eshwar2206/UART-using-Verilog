# UART using Verilog

**UART-using-Verilog** is a project that implements a Universal Asynchronous Receiver/Transmitter (UART) protocol using SystemVerilog. This repository provides the core modules for UART transmission and reception, along with a testbench for simulation and verification.

---

## Overview

**UART** is a widely-used serial communication protocol that enables the transfer of data between devices over a single serial line. This project simulates the key components of a UART system:

- **Transmitter**: Converts parallel data to a serial bit stream for transmission.
- **Receiver**: Converts incoming serial data back into parallel form.
- **Testbench**: Simulates UART communication and verifies correct operation.

---

## Repository Structure

| File             | Description                                      |
|------------------|--------------------------------------------------|
| `transmitter.sv` | UART transmitter module (serializes data)         |
| `receiver.sv`    | UART receiver module (deserializes data)          |
| `UART_TB.sv`     | Testbench for simulating and verifying UART       |
| `README.md`      | Project documentation                             |

---

## Features

- **8-bit Data Transmission**: Supports standard 8-bit UART communication.
- **Start and Stop Bits**: Implements UART framing for reliable data transfer.
- **Simulation Ready**: Includes a SystemVerilog testbench for functional verification.
- **Modular Design**: Separate transmitter and receiver modules for easy integration.

---

## Getting Started

### Prerequisites

- SystemVerilog-compatible simulator (e.g., ModelSim, VCS, Icarus Verilog)
- Basic understanding of Verilog/SystemVerilog and digital design

### Usage

1. **Clone the repository:**
   git clone https://github.com/eshwar2206/UART-using-Verilog.git
cd UART-using-Verilog

2. **Simulate the Testbench:**
- Open your preferred simulator.
- Compile `transmitter.sv`, `receiver.sv`, and `UART_TB.sv`.
- Run the simulation using the testbench (`UART_TB.sv`).
- Inspect the waveforms to verify that transmitted data matches received data.

---

## Module Descriptions

- **transmitter.sv**:  
Implements the logic to serialize 8-bit parallel data with start and stop bits for UART transmission.

- **receiver.sv**:  
Deserializes incoming UART data, detects start and stop bits, and outputs parallel data.

- **UART_TB.sv**:  
Stimulates the transmitter and receiver, checks data integrity, and provides waveform outputs for debugging.

---

## Customization

- **Baud Rate**:  
Adjust the timing parameters within the modules to match your target baud rate and system clock.

- **Data Width**:  
The modules are designed for 8-bit data, but can be modified for different data widths if required.



