# 안녕하세요 
![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white) ![Embedded](https://img.shields.io/badge/Embedded-000000?style=flat&logo=embedded&logoColor=white) ![Firmware](https://img.shields.io/badge/Firmware-4G4G4G?style=flat) ![STM32](https://img.shields.io/badge/STM32-032347?style=flat&logo=stmicroelectronics&logoColor=white)

.
# Hi, I'm Ganghyeon You 👋

Embedded/Firmware Developer focused on real-time control and reliable communication protocols.  
I like digging into why a system fails before I trust that it works — measuring, comparing, and rebuilding until the numbers back up the design.

---

## 🛠️ Tech Stack

### MCU & Platforms
<p>
  <img src="https://img.shields.io/badge/STM32F4-003B46?style=flat-square&logo=stmicroelectronics&logoColor=white"/>
  <img src="https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white"/>
  <img src="https://img.shields.io/badge/TI_MCU-0047AB?style=flat-square&logo=texas-instruments&logoColor=white"/>
  <img src="https://img.shields.io/badge/Xilinx_Zynq--7000-FF6B00?style=flat-square&logo=xilinx&logoColor=white"/>
</p>

### Communication Protocols & Tools
* **Protocols:** CAN, UART, SPI, I2C, iBus (RC telemetry)
* **Tools:** STM32CubeIDE, Verilog, Keil, Logic Analyzer, Oscilloscope

### Core Concepts
* DMA / Interrupt-driven design
* PID Control & FSM design
* Fail-safe design
* Bootloader (Basic)

---

## 🚀 Projects (2024 → 2026)

### 🔋 Integrated Vehicle Logging System (Formula Competition, 2025)
> **Role:** Electronics Team Lead  
> **Key Achieve:** Replaced subjective driver feedback with objective telemetry data, achieving zero packet loss.

* **Dual-MCU Architecture:** Designed a redundant Master/Slave system (Master: CAN capture & display / Slave: I2C receive & SD logging) to eliminate response delays caused by SD card write latency under a 10kW power limit.
* **Hardware Debugging:** Implemented a low-pass filter for gear-shift chattering and an OP-amp buffer circuit to resolve SAR ADC sampling errors on the suspension sensor.
* **Data-Driven Tuning:** Identified wheel-slip zones from logged data and collaborated with the mechanical team to optimize the suspension setup.
* **Team Mentorship:** Conducted workshops on wiring diagrams, relay usage, and feedback control basics to improve the team's Bus Factor.

---

### 🚁 STM32-based Drone Flight Controller (2026)
> **Role:** Personal Project  
> **Key Achieve:** Performance profiling and architecture refactoring for enhanced communication reliability.

* **DMA Optimization:** Profiled CPU occupancy using a logic analyzer; migrating from LL SPI Polling to HAL SPI DMA resulted in a **~50% CPU time reduction (143µs → 70µs)**.
* **Bug Fix (Data Corruption):** Traced an intermittent UART-interrupt data corruption bug to a local variable's lifetime and resolved it via static/global scoping.
* **Fail-safe Handling:** Designed a custom telemetry packet format and fail-safe routines for low battery and RC signal loss scenarios.

---

### 🎮 FPGA-based Tetris (2026)
> **Role:** Team Project (ZedBoard / Xilinx Zynq-7000)  
> **Key Achieve:** Hardware-level game logic design with zero-cycle delay.

* **FSM Modeling:** Modeled the entire game logic into a strict 4-state Finite State Machine (`SPAWN` → `FALL` → `MERGE` → `CLEAR`).
* **Zero-Delay Collision:** Implemented collision detection entirely in combinational logic for instant response.
* **Modular Independence:** Separated pixel-coordinate and block-coordinate systems to ensure high module independence.

---

### 🔌 Wiring Harness Redesign (Formula Car, 2024)
> **Role:** Electronics Team Member  
> **Key Achieve:** Enhanced reliability and reduced vehicle weight.

* **Weight Reduction:** Redesigned the overall harness layout, successfully reducing the total weight from **2.5kg to 2.0kg**.
* **Thermal Protection:** Rerouted critical wiring away from exhaust heat sources to prevent insulation damage and short circuits.
* **Vehicle Electronics Experience:** Gained practical knowledge of automotive relay operations, electrical noise isolation, and internal combustion engine control systems.

---
