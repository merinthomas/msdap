##Mini-Stereo Digital Audio Processor for EE6306 (ASIC Design)

### Introduction
Most of the modern multimedia systems require the implementation of audio processors which are highly accurate and efficient being the first priority. In order to achieve this, the cost becomes invariantly high. So, when the same design is to be used for portable devices or household applications such as audio systems, cost of the audio processor and power consumption are of major concern. Most of the similar audio processing designs are implemented using the Digital Signal Processing (DSP) chips with separate left and right channel processing that performs the basic function of Finite Impulse Response (FIR) Digital Filter. These filters will invariably involve multiplications. Implementing hardware multiplication, either floating or fixed point, is very costly with regard to power, area and complexity. We overcome these issues by replacing the multiplication unit with a one bit shifter and either an addition/subtraction unit which proves to be much faster and efficient than the former.

The system has been designed from specifications to RTL to physical design, taking it through the entire ASIC design flow.
* We have used structural Verilog HDL to represent the system
* Logic synthesis using Synopsys Design Compiler
* Physical design (Place & Route and timing analysis) using Synopsys IC Compiler

### Description and Usage of Files
* There are two versions of the full Verilog design - one in behavioral style (MSDAP_Behavioral.v) and the other in structural RTL style (MSDAP_RTL.v). Both are equivalent in functionality.
* There is a Verilog testbench file (Testbench.v) which feeds the input values and gathers output values.
* There is a data1.in file, which contains vectors for coefficient and input data values, to be used in the testbench to simulate the design.
* The data_expected1.out file contains the expected output vectors when data1.in is given as input to the design. It is used for functional verification purposes.
 
##### For further details, please refer the project report document (Final Report.docx)
