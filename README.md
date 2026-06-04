# 8-Bit Arithmetic Operations Using 8051
## Aim:
To perform 8-bit arithmetic operations such as addition, subtraction, multiplication, and division using the 8051 microcontroller.
## Apparatus Required:
Laptop with Keil uVision software
## Algorithm:
## For Addition:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Add the contents of registers A and B.
4.	Store the result in memory location 40H.
5.	Store the carry (if any) in 41H.
## For Subtraction:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Subtract B from A.
4.	Store the result in memory location 40H.
## For Multiplication:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Multiply A and B.
4.	Store the lower byte of the result in memory location 40H.
5.	Store the higher byte of the result in memory location 41H.
## For Division:
1.	Load the dividend from memory location 30H into register A.
2.	Load the divisor from memory location 31H into register B.
3.	Divide A by B.
4.	Store the quotient in memory location 40H.
5.	Store the remainder in memory location 41H.
## Programs:
```
ORG 0000H
MOV R1,#30H
MOV R2,#20H
MOV A,R1

ADD A,R2
MOV R4,A
CLR C

MOV A,R1
SUBB A,R2
MOV RS,A

MOV A,R1
MOV B,R2
MUL AB
MOV R6,A

MOV A,R1
MOV B,R2
DIV AB
MOV R7
```
## Output:
The results of addition, subtraction, multiplication, and division operations will be stored in memory locations 40H and 41H as specified in the program.
<img width="1552" height="821" alt="Screenshot 2025-10-24 133306" src="https://github.com/user-attachments/assets/3ef187fe-263b-47d5-8068-73dde44940aa" />

## Result:
The 8-bit arithmetic operations using the 8051 microcontroller have been successfully executed and verified using Keil software.


