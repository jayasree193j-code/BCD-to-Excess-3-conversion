# BCD to Excess-3 Converter

## Description
This project implements a BCD (Binary Coded Decimal) to Excess-3 code converter using Verilog HDL.

## Objective
The objective is to convert a 4-bit BCD input into its corresponding 4-bit Excess-3 output.

## Conversion Rule
Excess-3 code is obtained by adding 3 (0011) to the BCD input.

## Truth Table

| Decimal | BCD  | Excess-3 |
|---------|------|----------|
| 0       | 0000 | 0011     |
| 1       | 0001 | 0100     |
| 2       | 0010 | 0101     |
| 3       | 0011 | 0110     |
| 4       | 0100 | 0111     |
| 5       | 0101 | 1000     |
| 6       | 0110 | 1001     |
| 7       | 0111 | 1010     |
| 8       | 1000 | 1011     |
| 9       | 1001 | 1100     |

## Files

- `bcd_to_excess3.v` - Verilog design code
- `bcd_to_excess3_tb.v` - Testbench
- `output.vcd` - Simulation waveform file

## Software Required

- Icarus Verilog
- GTKWave
- GitHub

## How to Run

Compile the Verilog code:

    iverilog -o bcd_sim bcd_to_excess3.v bcd_to_excess3_tb.v

Run the simulation:

    vvp bcd_sim

Open the waveform:

    gtkwave output.vcd

## Expected Result

The output should be the Excess-3 representation of the valid BCD input from 0 to 9.

## Conclusion

The BCD to Excess-3 converter successfully converts each valid BCD digit into its corresponding Excess-3 code.
