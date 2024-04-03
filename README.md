### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/9078b4cd-1040-497d-9db4-6208c45b323b)



Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/f2fdb399-9196-4d5d-910e-8f08ff470453)



The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/6493d9ad-86cf-4d49-ab1a-702243a65334)


Figure 02  Encoder 8 * 3

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**PROGRAM**

Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: karthick v

RegisterNumber: 212223040086
```
module encoder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling:**

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/614a7556-3b27-4557-b6e4-b288a22ee9e6)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling:**

![image](https://github.com/gorghs/ENCODER8TO3DATAFLOW/assets/149037461/e94bfdbc-b63f-4b32-9751-a28b7540acef)


**RESULTS**

Therefore the code has been successfully executed.



