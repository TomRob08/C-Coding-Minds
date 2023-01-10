# While loop

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
