# FPGA Comparator
 
## Objective:
Use VHDL to design a 2-bit comparator and implement it on an FPGA chip on a Basys3 board. Then test proper functionality of the circuit. The FPGA board's slide switches should be used for inputting two 2-bit numbers, and the comparator outputs, three of them, should be mapped to any three LEDs available on the board.

## Testing:
The initial test of the source code was to ensure that it could successfully be used for a synthesis, implementation, and bitstream. The source code did not pass on the first attempt, so it was modified using suggestions from the Vivado log until a bitstream could successfully be generated.

Once the code had compiled successfully, I tested it by running it on a Basys 3 FPGA development board. The sixteen possible combinations of the four inputs were tested in the following manner. I utilized the binary numbers from 0 to 15. Each number correlated to a possible test case. For example, 0 corresponded to a False position for each switch and 1 corresponded to a value of True for the rightmost switch only. This method allowed me to efficiently cycle through each test case without missing or repeating any.

