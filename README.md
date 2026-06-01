## ⏱ 2-bit Synchronous Counter Design

The counter was implemented using two custom CMOS JK Flip-Flops.

### Counter Operation

The circuit is a 2-bit synchronous modulo-4 binary counter. Both flip-flops are driven by the same clock signal, ensuring that all state transitions occur simultaneously on the active clock edge.

The counter cycles through the following sequence:

00 → 01 → 11 → 00 → ...

State transition table:

| Current State | Next State |
|--------------|------------|
| 00 | 01 |
| 01 | 11 |
| 11 | 00 |


### State Diagram

![state_diagram](images/state_diagram.png)

### Schematic

![counter_schematic](images/counter_schematic.png)

### Layout

![counter_layout](images/counter_layout.png)

### Functional Simulation

![counter_waveform](images/counter_waveform.png)
