### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/c21f0e9c-5aee-4ad3-88aa-c95350fda59d)


Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/e4dcfd64-5a50-4129-a974-88317b8c06cf)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/9f03faf8-e214-4c16-a240-d026e02a0ac7)


Figure 02  Encoder 8 * 3

**Procedure**

write all the steps invloved 

**PROGRAM**

Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

**Encoder**
```
module encoder_top(din, a, b, c); 
input [0:7] din; 
output a,b,c; 
assign a=din[4] | din[5] | din[6] | din[7]; 
assign b=din[2] | din[3] | din[6] | din[7];
assign c=din[2] | din[4] | din[6] | din[7];
endmodule
```
Developed by: karthick v

RegisterNumber: 212223040086

**Output**

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/f1b54b7c-5216-4aa8-9c3b-00ea0ea596d6)




**RESULTS**

It is verified successfully.




