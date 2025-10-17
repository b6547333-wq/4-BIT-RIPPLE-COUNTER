# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

Open Quartus software and create a new Verilog file. Paste the code and save it. Compile the program to check for errors. Generate the RTL schematic via the RTL Viewer and save the logic diagram. Use the Waveform Editor to assign nodes for clk, rstn, and out. Simulate the design with different clk and rstn combinations to generate the timing diagram, and save the results.

**PROGRAM**

module ex12(out,clk,rst); input clk,rst; output reg [3:0]out; always @ (posedge clk) begin if(rst) out<=0; else out <= out-1; end endmodule

 Developed by:Thiru subramania sami  RegisterNumber:25000201

**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="579" height="336" alt="image" src="https://github.com/user-attachments/assets/12c8dff5-9776-443d-aea2-97ef82557000" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="826" height="476" alt="image" src="https://github.com/user-attachments/assets/7b336413-e8f4-4939-9890-8fc392bd7e66" />

**RESULTS**
implement 4 bit synchronous up counter and validate functionality
