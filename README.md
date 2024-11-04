# BOOLEAN_FUNCTION_MINIMIZATION
### NAME : Jayagar. T
### REG NO : 24901219
### EXPERIMENT 2 : BOOLEAN FUNCTIONS 

### AIM

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

### EQUIPMENTS REQUIRED

Hardware – PCs, Cyclone II , USB flasher

### SOFTWARE – QUARTUS PRIME

### THEORY

### LOGIC DIAGRAM
![Screenshot 2024-11-04 163706](https://github.com/user-attachments/assets/b6d05f6d-a885-4818-bfa7-5fb136d31c24)
![Screenshot 2024-11-04 164138](https://github.com/user-attachments/assets/1d63321e-b063-41fe-a93d-0d70092ad2ca)


### PROCEDDURE

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


### PROGRAM

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

#### Developed by: RegisterNumber:*/
#### module booleanfunction(a,b,c,d,F1,F2,w,x,y,z);
#### input a,b,c,d,w,x,y,z;
#### output F1,F2;
#### wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
#### assign x1=(~a)&(~b)&(~c)&(~d);
#### assign x2=(a)&(~c)&(~d);
#### assign x3=(~b)&(~c)&(~d);
#### assign x4=(~a)&(b)&(c)&(d);
#### assign x5=(b)&(~c)&(d);
#### assign x6=(x)&(~y)&(z);
#### assign x7=(~x)&(~y)&(z);
#### assign x8=(~w)&(x)&(y);
#### assign x9=(w)&(~x)&(y);
#### assign x10=(w)&(x)&(y);
#### assign F1=x1|x2|x3|x4|x5;
#### assign F2=x6|x7|x8|x9|x10;
#### endmodule


### RTL OUTPUT
![Screenshot 2024-11-04 103325](https://github.com/user-attachments/assets/e12feeba-9f49-49c8-9aee-e177f17a1c42)

### OUTPUT WAVEFORM
![Screenshot 2024-11-04 112947](https://github.com/user-attachments/assets/595f1616-00a5-4d92-84bc-c518ac61c106)



### RESULT

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

