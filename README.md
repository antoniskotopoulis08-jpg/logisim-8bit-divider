# 8-bit / 3-bit Sequential Divider — Logisim Evolution

A digital-logic project designed in **Logisim Evolution** for **Digital Logic Design at the National Technical University of Athens (NTUA)**.

The project implements an **unsigned 8-bit dividend / 3-bit divisor sequential divider** using an iterative, restoring-division-style datapath. The top-level circuit produces an **8-bit quotient** and a **4-bit remainder**.

## Project file

- `assignment.circ` — complete Logisim Evolution project
- Designed for **Logisim Evolution 4.0.0**
- Entry point: **`main`**

## Design overview

The `main` circuit combines arithmetic, storage, selection, and iteration-control logic to carry out the division over repeated clock cycles.

The active top-level design uses:

- **`AD_4BIT`** — 4-bit add/subtract block built from 1-bit full adders
- **`CNT`** — iteration counter used to track progress through the division
- **`FIND_Q`** — quotient-selection/update logic
- **`FIND_A`** — partial-remainder selection/update logic
- Shift-register, multiplexer, decoder, flip-flop, splitter, and gate-level components in the top-level datapath

The project file also retains supporting and developmental subcircuits created while building the design, including:

- `DFF_from_JK`
- `AD_1BIT`
- `shift`
- `DIVISOR_3BIT`
- `ADD_4BIT`
- `CTRL_FSM`
- `ctrl_fsm2`
- `ctrl_fsm3`
- `DATAPATH`
- `NEW_SHIFT`

These additional circuits document the iterative design process; the **`main`** circuit is the project entry point.

## Top-level interface

From the Logisim project definition, the main circuit includes:

- an **8-bit input** for the dividend
- a **3-bit input** (`M`) for the divisor
- a **RESET** input
- clock/control logic
- an **8-bit output** for the quotient
- a **4-bit output** for the remainder

## How to open

1. Install **Logisim Evolution 4.0.0** or a compatible newer version
2. Clone or download this repository
3. Open `assignment.circ`
4. Select the **`main`** circuit
5. Use Logisim's simulation tools to set the inputs and step/run the clock

## What this project demonstrates

- Hierarchical digital-circuit design
- Ripple-carry addition
- Two's-complement subtraction
- Sequential datapaths
- Shift-register based arithmetic
- Flip-flop based storage
- Counter and control logic
- Quotient and partial-remainder update logic
- Implementation of an iterative binary division algorithm in hardware

## Course

**National Technical University of Athens (NTUA)**  
Electrical & Computer Engineering  
Digital Logic Design — 2026

## Author

**Antonis Kotopoulis**

- GitHub: https://github.com/antoniskotopoulis08-jpg
- LinkedIn: https://www.linkedin.com/in/antonis-kotopoulis-6b5739411/

## Academic integrity

This repository is published as a personal portfolio and educational reference. If you are taking a similar course, do not submit this project or parts of it as your own coursework.
