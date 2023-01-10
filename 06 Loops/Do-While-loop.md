# Do/while loop
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
