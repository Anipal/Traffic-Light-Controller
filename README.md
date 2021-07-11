# Traffic-Light-Controller
In this project, we propose a design a modern FPGA-based traffic light control system to manage
road traffic. The approach is by controlling the access to different areas shared among multiple
intersections and allocating time between various users, during peak hours and off peak hours.
The main idea about this project is to manage the traffic movement of four intersecting roads and
to achieve optimum use of this traffic.

# Basic Methodology

The Finite State Machine is the key to the traffic light control system. It responds to the input
signals processed by the input handling model and provides the output and control signals
needed to make the system function. This design uses a standard two process FSM where one
process is used to change states on every clock cycle while the other process is used to calculate
the next state based on the current inputs and states. There are two types of state machines:
Mealy machine and Moore machine. In Mealy Machine, the output values are dependent on the
current state and the input values. In the Moore Machine, the output values solely depend on the
current state.
Two roads are considered opposite to each other with 5 possible states. They are initial reset
mode, so that state S0 shows red on both signals. After a certain time period, moving to state1,
signal on 1 side goes to red and other goes to green. And again up to a certain time count, it
changes from red and yellow and then moves to state 3 where the lights change to red. A similar
process takes place for remaining states

# Tools and Technology

Code is written in Verilog HDL and the synthesis is done on XILIX
