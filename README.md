![Tag](https://img.shields.io/badge/VLSI-Design-blue)
![Tag](https://img.shields.io/badge/DRAM-4x4-green)
![Tag](https://img.shields.io/badge/LTSpice-Simulation-orange)
![Tag](https://img.shields.io/badge/CMOS-180nm-red)
![Tag](https://img.shields.io/badge/Memory-Design-yellow)
![Tag](https://img.shields.io/badge/SenseAmplifier-NOT--Gate-lightgrey)
![Tag](https://img.shields.io/badge/Decoder-2x4-purple)
![Tag](https://img.shields.io/badge/DFF-RowBuffer-brightgreen)
![Tag](https://img.shields.io/badge/Status-Working-success)

# 4×4 DRAM Design — VLSI Final Project

This repository contains the complete LTSpice implementation, simulation files, and documentation for a semi‑realistic **4×4 DRAM** designed as part of the VLSI Design course. The project includes transistor‑level DRAM cells, decoders, sense amplifiers, row buffers, and a control FSM that performs full DRAM read, write‑back, and refresh operations.

---

## 📘 Project Overview

This project implements a functional **4×4 DRAM array** using:

- 1T DRAM cell (transistor + capacitor)
- 2‑to‑4 row decoder
- 2‑to‑4 column decoder
- NOT‑gate‑based sense amplifiers
- CMOS D flip‑flops as row buffers
- Control FSM for sequencing read/write/refresh operations

The design follows the required DRAM read sequence and demonstrates correct timing behavior in the **nanosecond range**.

---

## 🚀 Features

- ✔ Fully functional 4×4 DRAM array  
- ✔ Destructive read + automatic write‑back  
- ✔ Row buffer using CMOS DFFs  
- ✔ Sense amplifiers using NOT gates  
- ✔ FSM‑based control logic  
- ✔ Refresh after every 5 operations  
- ✔ LTSpice simulations with 1 fF load  
- ✔ 180 nm technology, VDD = 1.8 V  
- ✔ 10 ps rise/fall times  
- ✔ Includes all simulation outputs (.raw, .op, .plt)  
- ✔ Includes full project report (PDF + DOCX)  

---

## 📂 Repository Structure
│── DRAM.asc               # Main 4×4 DRAM schematic
│── Dff.asc                # CMOS D flip-flop (row buffer)
│── NAND.asc / NAND3.asc   # Logic gates used in decoders
│── NOT.asc                # Sense amplifier
│── SA.asc                 # Sense amplifier block
│── smux.asc               # Column multiplexer
│── Demux2-4*.asc          # Row decoder variants
│── *.asy                  # LTSpice symbol files
│── *.op / *.raw / *.plt   # Simulation outputs


---

## 📊 Simulation Requirements

All simulations follow the project constraints:

- Technology: **180 nm**
- VDD: **1.8 V**
- Load capacitance: **1 fF**
- Rise/Fall time: **10 ps**
- Screenshots include timestamp

---

## 🧪 Demonstrated Behavior

- Correct DRAM read sequence  
- Sense amplifier operation  
- Row buffer capture  
- Column selection  
- Write‑back after destructive read  
- Full refresh of all 4 rows  
- Measured read latency in nanoseconds  

---

## 📄 Report


## ▶ How to Run

1. Open `.asc` files in **LTSpice**  
2. Ensure `.asy` symbol files are in the same directory  
3. Run simulations directly  
4. View waveforms in `.raw` files  

---


