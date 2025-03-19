# Simple Voting Machine

## Project Overview
This project is a digital voting machine designed using FPGA technology and Vivado software. The system enables voters to select from a set of options using physical buttons and displays the results via LEDs. It integrates both combinational and sequential logic to register votes, showcase results, and reset for future voting sessions.

## Project File Name
**Simple_Voting_Machine**

## Objective
The aim of this project is to develop a reliable and efficient voting system using FPGA technology to:
- Register valid votes using a debounced button mechanism.
- Count and tally votes securely.
- Display voting results using LED indicators.
- Provide a reset function for new voting sessions.

## Technologies Used
- **Vivado software tool**
- **ZED Board (FPGA hardware)**

## System Components
1. **Voting Interface**  
   - Buttons for voters to select options.  
   - Debouncing mechanism to ensure accurate input.

2. **Vote Processing Unit**  
   - Combinational logic for decoding button inputs.  
   - Sequential logic to manage the voting process state.

3. **Vote Counting and Tallying**  
   - Counters for tracking votes.  
   - Registers for secure vote storage and real-time updates.

4. **Result Display**  
   - LEDs to visually indicate the number of votes received for each option.

5. **Control and Reset Mechanism**  
   - A dedicated reset button for system reinitialization.

## System Operation
1. **Initialization**  
   - System powers up with all counters and registers set to zero.  
   - LEDs are turned off to indicate no votes have been cast.

2. **Voting Process**  
   - Voters press the buttons corresponding to their preferred options.  
   - Debouncing logic ensures accurate registration of button presses.  
   - Counters increment for each valid vote.

3. **Vote Counting**  
   - Registers update in real-time with the vote counts.

4. **Result Display**  
   - LEDs display the number of votes for each candidate.

5. **Resetting the System**  
   - Pressing the reset button clears all counters and prepares the system for the next voting session.

## Code Structure
- **Mode Control Module:** Handles vote counting and LED display control.
- **Vote Logger Module:** Maintains a record of votes per candidate.
- **Button Control Module:** Ensures accurate button press detection through debouncing.
- **Main Voting Machine Module:** Integrates all components for complete functionality.

## How to Run
1. Install **Vivado** software.
2. Load the provided VHDL code into Vivado.
3. Connect the ZED Board and program it with the generated bitstream.
4. Use the buttons to cast votes and observe the LED result display.

## Contributors
- **CH K Vardhan**  
- **D Harsha Vardhan**  
- **N Prasanna**

## Faculty Incharge
- **Dr. Navya Mohan**  
- **Dr. Bala Tripura Sundari B**

## License
This project is intended for educational purposes and follows open-source guidelines.

