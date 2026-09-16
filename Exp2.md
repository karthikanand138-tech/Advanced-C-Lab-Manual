EXP NO:2 C PROGRAM FOR PASSING STRUCTURES AS FUNCTION ARGUMENTS AND RETURNING A STRUCTURE FROM A FUNCTION
Aim:
To write a C program for passing structure as function and returning a structure from a function

Algorithm:
1.	Define structure numbers with members a and b.
2.	Declare variable n of type numbers.
3.	Prompt the user to enter values for a and b.
4.	Input values for a and b into n using scanf.
5.	Call the add function with n as an argument.
6.	Print the result returned by the add function.
7.	Return 0
 
Program:

```
#include <stdio.h>

struct Data
{
    int a;
    int b;
};

struct Data addStructs(struct Data d1, struct Data d2)
{
    struct Data result;

    result.a = d1.a + d2.a;
    result.b = d1.b + d2.b;

    return result;
}

int main()
{
    struct Data d1, d2, result;

    scanf("%d %d", &d1.a, &d1.b);
    scanf("%d %d", &d2.a, &d2.b);

    result = addStructs(d1, d2);

    printf("%d %d", result.a, result.b);

    return 0;
}

```




Output:

<img width="477" height="395" alt="image" src="https://github.com/user-attachments/assets/85fa510d-8d03-405f-977d-df923d756523" />



Result:
Thus, the program is verified successfully
