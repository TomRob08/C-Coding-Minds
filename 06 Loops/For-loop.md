# For loop
A for loop is used when you know how many times a block of code should repeat.

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  for(int i = 0; i < 5; i++)
  {
    cout << i << endl;
  }
  return 0;
}
```

### Output:
```
0
1
2
3
4
```

Let me explain each statement inside the parentheses of the for loop.

- ```int i = 0;```: Initializes a variable to be used inside of the for loop. This variable cannot be used outside of the for loop.
- ```i < 5;```: This is the condition that will be checked each time it loops.
- ```i++```: Increments ```i```. Decrementing can also be done here if ```i++``` is replaced with ```i--```. If you would like to change the value of ```i``` by more than 1, you would use ```i+=2``` to increase the value by 2 or you can use any other number you'd like instead of 2 and it would increase ```i```'s value by that number. Decreasing is done in a similar way such as ```i-=2```.

### Exercises:
__1.__ Ask a user to enter 2 different letters with the first letter being before the second letter in the alphabet. Then print all of the letters between the two using a for loop with the user letters included. (Type casting would be useful for this and look up the ascii table as a reference).

__2.__ Create a program to produce the factorial of any number.
