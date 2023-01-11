# Nested Loops

A nested loop is a loop inside another loop. The main idea is that the "inner loop" will be executed one time for each iteration of the "outer loop". In other words, for each iteration of an outer loop the inner loop re-starts and completes its execution before the outer loop can continue to its next iteration. Nested loops can be used with for loops, while loops, or a combination of both.

## Nested For Loop

### Example:
```
#include <iostream>
using namespace std;

int main() 
{
  for (int i = 0; i < 5; i++)
  {
    for (int j = 0; j < 5; j++)
    {
      cout << "(i:" << i << ", j:" << j << ") ";
    }
    cout << endl;
  }
}
```

### Output:
```
(i:0, j:0) (i:0, j:1) (i:0, j:2) (i:0, j:3) (i:0, j:4) 
(i:1, j:0) (i:1, j:1) (i:1, j:2) (i:1, j:3) (i:1, j:4) 
(i:2, j:0) (i:2, j:1) (i:2, j:2) (i:2, j:3) (i:2, j:4) 
(i:3, j:0) (i:3, j:1) (i:3, j:2) (i:3, j:3) (i:3, j:4) 
(i:4, j:0) (i:4, j:1) (i:4, j:2) (i:4, j:3) (i:4, j:4)
```

## Nested While Loop

### Example:
```
#include <iostream>
using namespace std;

int main() 
{
  int i = 0;
  while (i < 5)
  {
    int j = 0;
    while (j < 5)
    {
      cout << "(i:" << i << ", j:" << j << ") ";
      j++;
    }
    i++;
    cout << endl;
  }
}
```

### Output:
```
(i:0, j:0) (i:0, j:1) (i:0, j:2) (i:0, j:3) (i:0, j:4) 
(i:1, j:0) (i:1, j:1) (i:1, j:2) (i:1, j:3) (i:1, j:4) 
(i:2, j:0) (i:2, j:1) (i:2, j:2) (i:2, j:3) (i:2, j:4) 
(i:3, j:0) (i:3, j:1) (i:3, j:2) (i:3, j:3) (i:3, j:4) 
(i:4, j:0) (i:4, j:1) (i:4, j:2) (i:4, j:3) (i:4, j:4)
```

## Exercises
__1.__ Create a square using nested loops that looks like this:
```
*****
*****
*****
```

__2.__ Create a triangle using nested loops that looks like this:
```
*
**
***
****
```

__3.__ Use nested loops to produce the output below. (Hint: Two separate inner loops may help)
```
0  1  2  3  4  
1  0  1  2  3  
2  1  0  1  2  
3  2  1  0  1  
4  3  2  1  0 
```
