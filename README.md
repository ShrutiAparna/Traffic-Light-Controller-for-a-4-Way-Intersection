**Introduction:**
<p>This project presents the design and implementation of a traffic light controller for a 4-way intersection using Verilog. The system aims to regulate traffic flow and enhance road safety by controlling the sequence of traffic lights at the intersection. The Verilog code simulates the behavior of the traffic lights based on predefined timing sequences. Simulation results demonstrate the proper functioning of the traffic light controller in various traffic scenarios.</p>

**Inspiration:**
<p>Traffic lights play the most important role in our lives while dealing with huge traffic and an increasing population. This controller system is used to design the Traffic lights with the concept of a 4-way road system.</p>

**Application:**
<p>Traffic management is crucial for ensuring smooth traffic flow and preventing accidents at intersections. The controller governs the operation of traffic lights at a 4-way intersection, providing an efficient and safe traffic management solution.</p>


**Working of the circuit:**
<p>The code for a Traffic Light Controller uses a Finite State Machine (FSM) to control a four-way traffic intersection with north, south, east, and west directions. </p>
<p>- Inputs: “clk” (clock signal) and "rst_a" (reset signal).</p>
<p>- Outputs: 3-bit signals for lights in each direction ("n_lights", "s_lights", "e_lights", "w_lights").</p>

The FSM cycles through the following sequence of light states for each direction:
- Greenlight ("001") for 8 clock cycles.
- Yellow light ("010") for 4 clock cycles.
- Red light ("100") as the default state.
  
The FSM transitions between north, south, east, and west states in order, and the cycle repeats. On reset, the FSM starts in the north state.

**Designing The Circuit:**
<p>We will use JK Flip Flops to implement this mod-8 counter</p>

