# EX 1c Implementation of Tower of Hanoi
## DATE:26-2-25
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1.	Start the program.
2.	Check if n is greater than 0.
3.	Recursively move n-1 disks from source (x) to auxiliary (z) using destination (y).
4.	Print the move of the n-th disk from source (x) to destination (y).
5.	Recursively move n-1 disks from auxiliary (z) to destination (y) using source (x).
6.	The function is called initially with TOH(n, 'A', 'B', 'C') where 'A', 'B', and 'C' are the rods.
7.	End

  

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: HARSSHITHA LAKSHMANAN
RegisterNumber:  212223230075
*/
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
if(n>0)
{
TOH(n-1,x,z,y);
printf("%c to %c",x,y);
printf("\n");
TOH(n-1,z,y,x);
}
}
int main()
{
int n=2; TOH(n,'A','B','C');
}

```

## Output:


![image](https://github.com/user-attachments/assets/74af8a62-3c46-4490-a616-2c289e1a6ece)



## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
