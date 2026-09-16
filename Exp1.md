EXP NO:1 C PROGRAM FOR ARRAY OF STRUCTURE TO CHECK ELIGIBILITY FOR THE VACCINE.

Aim:
To write a C program for array of structure to check eligibility for the vaccine person age above 6 years of age.

Algorithm:
1.	Declare structure eligible with age (integer) and n (character array)
2.	Declare variable e of type eligible
3.	Input age and name using scanf, store in e
4.	If e.age <= 6
-	Print "Vaccine Eligibility: No"
Else
-	Print "Vaccine Eligibility: Yes"
5.	Print details (e.age, e.n)
6.	Return 0
 
Program:
```

#include <stdio.h>

struct Person
{
    char name[20];
    int age;
};

int main()
{
    struct Person p[10];
    int n, i;

    printf("Enter number of persons: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++)
    {
        printf("Enter name and age: ");
        scanf("%s %d", p[i].name, &p[i].age);
    }

    printf("\nVaccine Eligibility:\n");

    for(i = 0; i < n; i++)
    {
        if(p[i].age > 6)
            printf("%s - Eligible\n", p[i].name);
        else
            printf("%s - Not Eligible\n", p[i].name);
    }

    return 0;
}

```


Output:

<img width="516" height="257" alt="image" src="https://github.com/user-attachments/assets/1d873cd3-04e7-4de6-9b9a-c0b6e2ae15e0" />



Result:
Thus, the program is verified successfully.
