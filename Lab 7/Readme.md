#### Lab 7: VHDL Code for Sequential Circuits — Flip-Flops

### Objective
Design and simulate SR, D, JK, and T flip-flops using VHDL.
Understand the importance of the clock signal in sequential circuits.
Observe and compare the behavior of different types of flip-flops.


#### Theory

A flip-flop is a bistable sequential circuit that stores one bit of data. Unlike combinational circuits, the output of a flip-flop depends on both the current inputs and its previous state. Most flip-flops change their state only on the rising edge of the clock, making them fundamental building blocks of synchronous digital systems.

### SR Flip-Flop

The SR (Set-Reset) flip-flop is the simplest type of flip-flop. It provides separate inputs for setting and resetting the output.

S	R	Q (Next State)
0	0	No Change
0	1	0 (Reset)
1	0	1 (Set)
1	1	Invalid/Forbidden
### D Flip-Flop

The D (Data) flip-flop stores the value present at the D input when the clock edge occurs.

Equation:

Q
next
	​

=D

This flip-flop eliminates the invalid state found in the SR flip-flop, making it suitable for data storage applications.

### JK Flip-Flop

The JK flip-flop is an improved version of the SR flip-flop. It removes the forbidden state by allowing the output to toggle when both inputs are high.

###
# J	K	Operation
0	0	Hold
0	1	Reset
1	0	Set
1	1	Toggle
T Flip-Flop

The T (Toggle) flip-flop changes its output whenever T = 1 at the clock edge. When T = 0, the output remains unchanged.

Equation:

Q
next
	​

=T⊕Q

The T flip-flop is commonly used in counters and frequency division circuits.

### Output






#### Discussion


The clock signal ensures that state changes occur only at specific instants, providing synchronized operation.
The SR flip-flop demonstrates basic memory functionality but includes a forbidden input condition.
The D flip-flop simplifies circuit design by directly storing the input value on the clock edge.
The JK flip-flop removes the invalid state of the SR flip-flop and supports toggling, making it suitable for counters and control circuits.
The T flip-flop is a simplified toggle device that is widely used in frequency dividers and binary counters.
#### Conclusion


SR, D, JK, and T flip-flops were successfully designed and simulated using VHDL.
The simulation verified that all flip-flops change their states according to their respective truth tables on the active clock edge.
The experiment demonstrated the essential role of the clock signal in controlling sequential circuits.
Each flip-flop serves a different purpose:
SR Flip-Flop: Basic set and reset operations.
D Flip-Flop: Reliable one-bit data storage.
JK Flip-Flop: Flexible operation with toggle capability.
T Flip-Flop: Efficient implementation of counters and frequency dividers.
These flip-flops form the foundation of more advanced sequential circuits such as registers, counters, shift registers, and memory systems.
