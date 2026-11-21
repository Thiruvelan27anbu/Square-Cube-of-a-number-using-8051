# Square-Cube-of-a-number-using-8051
# 8051 Square  Program

## AIM
To write and execute an Assembly language program for finding the square of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value to Port 0 (P0).
3. Execute the program.
4. The output square value is stored in Port 2 (P2).
## flow cart 
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/f4dfd4a3-75e2-4822-b1f9-900795c177cc" />

## PROGRAM
```
ORG 0000H
MOV DPTR, #8100H
MOVX A, @DPTR
MOV B,A
MUL AB
MOV DPTR, #8102H
MOVX @DPTR,A
INC DPTR
MOV A,B
MOVX @DPTR,A
END

```

## OUTPUT
<img width="1600" height="830" alt="image" src="https://github.com/user-attachments/assets/4b8825ff-d605-4363-93c1-d4d1b9208498" />


## RESULT
Thus, the square of the given data is calculated using 8051 Keil.

# 8051 Cube  Program

## AIM
To write and execute an Assembly language program for finding the cube of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value.
3. Execute the program.
4. The output cube value is stored in a memory location.
## flow chart
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/2ef8bf1c-5b55-45ca-b57e-993556d1cfc3" />

## PROGRAM
```

ORG 0000H
MOV DPTR, #9000H
MOVX A, @DPTR
MOV B,A
MOV R1,A
MUL AB
MOV R2,B
MOV B,R1
MUL AB
MOV DPTR, #9003H
MOVX @DPTR,A
MOV R3,B
MOV B,R2
MOV A,R1
MUL AB
ADD A,R3
DEC DPL
MOVX @DPTR,A
MOV A,#00H
ADDC A,B
DEC DPL
MOVX @DPTR,A
HERE: SJMP HERE
END

```


## OUTPUT
<img width="1600" height="797" alt="image" src="https://github.com/user-attachments/assets/ad50e671-0c65-46e4-89fe-5734089875fe" />


## RESULT
Thus, the cube of the given data is calculated using 8051 Keil.


