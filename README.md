# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

FUNTION 1 K-MAP


![FUNTION 1 K-MAP](https://github.com/user-attachments/assets/25d455d9-0cdd-409a-9ecb-1226cd83aed2)


FUNTION 2 K-MAP


![FUNTION 2 K-MAP](https://github.com/user-attachments/assets/a3b74a66-6dee-4f9a-8c76-a3cbf657a176)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Program:**


```
 FUNCTION 1

 
 module function1(a,b,c,d,f1);
 input a,b,c,d;
 output f1;
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 endmodule

 
 FUCTION 2

 
 module funct2(w,x,y,z,f2);
 input w,x,y,z;
 output f2;
 assign f2=((~y & z)|( w & y )|(x & y));
 endmodule

```


FUNTION 1:



![FUNTION 1 TT](https://github.com/user-attachments/assets/72d8a4da-27ff-4108-888a-a17e0da96691)



FUNTION 2:



![FUNTION 2 TT](https://github.com/user-attachments/assets/b42a432b-91e2-4ab0-bdbe-72b19694f3ce)


**RTL realization**

**Output:**

**RTL**



FUNTION 1:


![Screenshot 2024-12-05 191614](https://github.com/user-attachments/assets/100f2d96-82d0-4778-b795-8bb82d5286b9)


FUNTION 2:



![Screenshot 2024-12-05 191718](https://github.com/user-attachments/assets/d4d11eab-4013-4af3-92d1-607e64498333)




**Timing Diagram**

FUNTION 1:


![Screenshot 2024-12-05 204243](https://github.com/user-attachments/assets/6a685563-6f36-4aa9-85ee-14672f4960de)


FUNTION 2:



![Screenshot 2024-12-05 204350](https://github.com/user-attachments/assets/90941dca-7de4-4030-b2ae-79d58ca93ac8)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

