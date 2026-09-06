# Circuit Inventory

The uploaded Logisim Evolution project contains the following circuits.

## Active top-level design

- **`main`** — project entry circuit. It directly instantiates `CNT`, `AD_4BIT`, `FIND_Q`, and `FIND_A`, together with Logisim shift-register, multiplexer, decoder, splitter, flip-flop, clock, and gate-level components.
- **`AD_4BIT`** — 4-bit add/subtract unit with a 4-bit `A` input, 3-bit `B` input, `SUB` control, 4-bit sum/result `S`, and `COUT`. It is built from four `AD_1BIT` blocks.
- **`AD_1BIT`** — reusable 1-bit full-adder building block.
- **`CNT`** — iteration counter/reset logic with a `LAST` output used by the sequential divider control.
- **`FIND_Q`** — 8-bit quotient selection/update logic.
- **`FIND_A`** — 4-bit partial-remainder selection/update logic.
- **`DFF_from_JK`** — D-type storage behaviour implemented from JK flip-flop logic and reused by the counter design.

## Additional / developmental circuits

The project file also retains subcircuits created during development and experimentation:

- `shift`
- `DIVISOR_3BIT`
- `ADD_4BIT`
- `CTRL_FSM`
- `ctrl_fsm2`
- `ctrl_fsm3`
- `DATAPATH`
- `NEW_SHIFT`

These are kept because they show the iterative design process. The circuit selected as the project entry point is **`main`**.

## Complete circuit list

1. `main`
2. `DFF_from_JK`
3. `AD_1BIT`
4. `AD_4BIT`
5. `shift`
6. `DIVISOR_3BIT`
7. `ADD_4BIT`
8. `CNT`
9. `CTRL_FSM`
10. `ctrl_fsm2`
11. `ctrl_fsm3`
12. `DATAPATH`
13. `FIND_Q`
14. `FIND_A`
15. `NEW_SHIFT`
