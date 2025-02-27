# Samsung-RISC-V-Program
RISC-V Internship program powered by SAMSUNG and VSD
This RISC-V Internship using VSDSquadron Mini is based on RISC-V architecture and uses open-source tools to teach students about VLSI SoC Design and RISC-V. The instructor and guide for this internship is Kunal Ghosh Sir, Founder of VSD.
Basic Details
Name: DIVYA.M
College: R V INSTITUTE OF TECHNOLOGY AND MANAGEMENT
Email ID:divyamallikarjun2020@gmail.com

Task 1 - Compilation Differences Between -O1 and -Ofast
-O1 Optimization
Prioritizes readable and understandable code with basic optimizations.
Larger number of instructions due to minimal optimization.
Keeps intermediate calculations and variables in memory.
Detailed code flow makes it easier to follow and debug.
-Ofast Optimization
Aggressive optimization for maximum performance, potentially sacrificing strict adherence to standards.
Fewer instructions as redundant operations are removed.
More compact code layout with streamlined computations.
Reduced intermediate steps, making the code harder to debug but faster to execute.

Task 2 - Optimization Flags -O1 and -Ofast Performance
-O1 Optimization
Takes longer route with more detailed steps.
Starts at memory address 0x10184.
More instructions and steps visible.
Easier to debug and follow the program flow.
Good for development and testing phase.
-Ofast Optimization
Takes shorter, faster route.
Starts at memory address 0x100b0.
Fewer instructions to do the same task.
Harder to debug but better performance.
Perfect for final production code.
Main Differences
Memory addresses are organized differently.
-Ofast uses fewer registers more efficiently.
Instruction count is lower in -Ofast.
Both reach the same result (e.g., 120) but through different paths.
Memory & Performance
-Ofast has a more compact code layout.
Better register management in -Ofast.
Less memory usage in the -Ofast version.
Faster execution due to optimization.
Trade-offs
O1: Better debugging vs slower performance.
Ofast: Better performance vs harder debugging.
-O1 shows a clear instruction flow.
-Ofast focuses on speed over readability.

Task 3 - Instruction Set Description
List of Commands
lui - Load Upper Immediate
addi - Add Immediate
li - Load Immediate
sd - Store Doubleword
jal - Jump and Link
ret - Return
ld - Load Doubleword
auipc - Add Upper Immediate to PC
beqz - Branch if Equal to Zero
j - Unconditional Jump
sub - Subtract
lbu - Load Byte Unsigned
bnez - Branch if Not Equal to Zero
sb - Store Byte
jr - Jump Register
mv - Move
jalr - Jump and Link Register

Task 4: Functional Simulation of RISC-V Core
Objective
Perform a functional simulation of the RISC-V Core Verilog netlist using a comprehensive testbench.

Environment Setup
Simulation Tools:
Icarus Verilog (iverilog)
GTKWave
Platform: Linux/Ubuntu
Simulation Procedure
File Preparation

Downloaded RISC-V Core Verilog Netlist
Obtained corresponding Testbench
Compilation Commands

iverilog -o simulation netlist.v testbench.v
./simulation
gtkwave waveform.vcd

Task 5: Radar System for Threat Detection
Project Overview
A surveillance system utilizing an ultrasonic sensor (HC-SR04) and VSD Squadron to detect potential threats within a specified range. The system provides visual feedback through LED indicators for threat detection status.

Functionality
Ultrasonic sensor emits pulse via Trig pin.
Echo pin receives reflected pulse for distance calculation.
Red LED activates when object detected within threshold.
Green LED indicates clear status when no threats detected

Task 6: Implementation and Video Demonstration
Objective
Successfully implement the Radar System on a RISC-V board and demonstrate its functionality via a video.

Steps to Implementation
Hardware Setup

Connected Ultrasonic Sensor, LEDs, and VSD Squadron as per circuit diagram.
Verified power connections and component placements.
Software Development

Wrote the embedded C code for distance measurement and LED control.
Uploaded the program to the RISC-V board.
Integrated threshold-based detection logic.
Testing and Debugging

Ran multiple test cases with varying object distances.
Verified LED responses for different distance thresholds.
Debugged minor sensor timing issues for accuracy.
Final Demonstration

Recorded a video showcasing the radar system in action.
Explained the system components, working, and test results in the video.
Uploaded the video as part of the final submission.
Key Takeaways
Successful implementation: Radar system functioned as expected.
Accurate threat detection: Red LED triggered within set range.
Optimized code execution: Efficient register usage ensured smooth operation.
Video demonstration completed: Showcased the real-time working of the project.
Conclusion
This task successfully demonstrated the ability to implement and test an embedded system on a RISC-V platform. The final video presentation validated the system's functionality and efficiency in detecting threats using an ultrasonic sensor.


