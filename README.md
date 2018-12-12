# Pipelined-Processor
Logisim implementation of 5-stage pipelined processor that runs the custom GT-2200 ISA

*__Bodamer_Pipeline_Logisim.circ__* contains the implementation of the processor

*__pow.s__* contains the test assembly program that runs on the processor. It computes the operation 2^10 and stores it into register $v0

*__pow.hex__* contains the same assembly instructions translated into hex so the processor can make use of them

## Intsructions for running:
Simulation runs using Logisim

pow.hex contains both the instructions and relevant data, so make sure the Insruction ROM and Data RAM both hold pow.hex

Look at the Simulate tab in the menu bar of Logisim. Change tick frequency as desired. 4.1 KHz is recommended if you just want to see the output.

Enable the simulation and look into the register file. $v0 should approach 0x400 (1024)
