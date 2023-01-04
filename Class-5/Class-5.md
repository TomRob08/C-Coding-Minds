# Class 5
## While loop

While loops repeat a block of code for the period of time that the condition is true.

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  int i = 0;
  
  while(i < 5)
  {
    cout << i << endl;
    i++;
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

As you can see in the example, the while loop ran and then stopped when ```i``` equaled 5.

### Exercises:
__1.__ Continuously ask a user for numbers in a loop and end the loop if the user enters 0. When the loop ends, print the sum of the given user numbers.

__2.__ Use a random variable between 0 and 100 and have a user guess the number in a loop. Let the user know if their guess is higher or lower than the actual number and when they get the number correct.

__Using random numbers example:__
```
#include <iostream>
#include <cstdlib>
#include <time.h>
using namespace std;

int main() {
  srand(time(0));
    
  cout << rand() % 100 << endl;

  return 0;
}
```
  
```srand()``` enables ```rand()``` to generate a different number each time. ```rand() % 100``` sets the upper bound and the lower bound is 0 by default. Make sure to have ```#include <cstdlib>``` and ```#include <time.h>```

## Do/while loop
A do/while loop works in a similar way as the normal wile loop but the condition is placed at the end after the last bracket with a semicolon and the word ```do``` is placed at the beginning

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  int i = 0;
  
  do
  {
    cout << i << endl;
    i++;
  } while(i < 5);
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

The difference between the do/while loop and the while loop is a do/while loop will run the block of code at least once before checking if the condition is true.

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  int i = 0;
  
  do
  {
    cout << i << endl;
    i++;
  } while(i == 5);
  return 0;
}
```

### Output:
```
0
```

In the exmple, the while condition is false but it still runs once because it didn't check the condition until after the block of code.

### Exercise:
__1.__ Use a do while loop and have a user enter data. The loop should continue as long as the data entered is a number and print what is inputted. Use ```isdigit()``` function to check if the data is a number and have ```#include <ctype.h>``` in your program.

## For loop
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

__2.__ 
