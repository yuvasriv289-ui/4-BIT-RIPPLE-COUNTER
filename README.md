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

1.Type the program in Quartus software.
2.Compile and run the program.
3.Generate the RTL schematic and save the logic diagram.
4.Create nodes for inputs and outputs to generate the timing diagram.
5.For different input combinations generate the timing diagram

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.
```
module EXP12DE(clk, rst, count);
input wire clk;
input wire rst;
output reg [3:0] count;

always @(posedge clk or posedge rst)
begin
	if(rst)
		count <= 4'b0000;
	else
		count <= count + 1;
end
```
endmodule

 Developed by:Yuvasri V
 RegisterNumber:25008890
*/

**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="1006" height="348" alt="527124022-291a3345-016e-4d14-a1f8-1da19730152c" src="https://github.com/user-attachments/assets/e0f83643-6717-47b9-84a4-12ecb215744b" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1367" height="780" alt="527124151-90fd3fb3-2c22-489b-8967-bde768d10b29" src="https://github.com/user-attachments/assets/0ef001c5-1e3c-4446-8586-869a4675d9ed" />

**RESULTS**
 The 4-bit ripple counter was successfully implemented using Verilog in Quartus Prime
