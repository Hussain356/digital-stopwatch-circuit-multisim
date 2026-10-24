# Digital Stopwatch Circuit (Multisim)

A digital stopwatch designed and simulated in NI Multisim, using TTL counter and decoder ICs to drive six seven-segment displays.

![Stopwatch circuit](Stop_Watch.png)

## Components
| Component | Qty | Role |
|---|---|---|
| 7490N decade counter | 6 | Counts clock pulses in BCD |
| 7447N BCD to seven-segment decoder | 6 | Converts BCD to display segments |
| Common-anode seven-segment display | 6 | Shows the digits |
| 74HC32 OR gate | 2 | Combines push-button input with the control logic |
| Push buttons (DPST) | 2 | Manual control of the counters |
| Function generator | 1 | Clock source |
| 5 V supply | 1 | Power |

## How it works
The function generator supplies clock pulses to the first 7490 counter. Each 7490 counts in BCD, its output feeds a 7447 decoder, and the decoder drives one seven-segment display. The six counter, decoder, and display stages are chained so each digit advances from the one before it.

## Run
1. Open the circuit file in NI Multisim.
2. Start the simulation.
3. Use the push buttons to control the count.

## Tools
NI Multisim, TTL logic ICs (7490, 7447), CMOS OR gate (74HC32).
