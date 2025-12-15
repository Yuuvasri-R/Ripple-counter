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

/* write all the steps invloved */

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by: Yuuvasri R
 RegisterNumber:25003422
*/
```
module Asy_Co (
    input  wire clk,       // clock input
    input  wire rst,       // synchronous reset
    output reg  [2:0] q   // 3-bit counter output
);

initial begin
     q <= 3'b0000;
	 end

always @(posedge clk) 
begin
q <= 3'b000;
    if (rst) 
        q <= 3'b000;       // reset counter to 0
    else
        q <= q - 1;        // increment counter
end

endmodule

```


**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="1871" height="760" alt="Screenshot 2025-12-15 121251" src="https://github.com/user-attachments/assets/be682933-4aa3-4bf8-a8be-0897f7b358dc" />


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1468" height="766" alt="image" src="https://github.com/user-attachments/assets/30360a7d-790f-497e-a9fe-17b7adf608eb" />

**RESULTS**
Thus implementing 4 Bit Ripple Counter using Verilog and validating their functionality using their functional tables is done successfully.


...



...




...






...
