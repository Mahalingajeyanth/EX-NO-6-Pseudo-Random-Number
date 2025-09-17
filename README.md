# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
1.Start the program and import the required libraries.

2.Seed the random number generator using the current time(i.e) rand(time(0));

3.Get the number of randon number to generate.

4.Pass the value for number of iterations and print the numbers.

5.End the program.

# PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }
    return 0;
}
```

# OUTPUT:
<img width="1679" height="865" alt="Screenshot 2025-09-17 092425" src="https://github.com/user-attachments/assets/db5df464-d61b-41ac-baad-86da7d3ff8f8" />


# RESULT:
Thus the given Pseudo-Random-Number program was successfully verified.
