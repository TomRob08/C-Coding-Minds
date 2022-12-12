# Class 3
## Boolean Comparisons
### Comparison Operators:
- ```==```: Equal to. Checks to see if the two values are the same.
- ```!=```: Not equal
- ```>```: Greater than
- ```<```: Less than
- ```>=```: Greater than or equal to
- ```<=```: Less than or equal to

### Examples:
```
#include<iostream>
using namespace std;

int main()
{
  cout << (10 == 10) << endl;
  cout << (10 == 0) << endl;
  cout << (0 != 10) << endl;
  cout << (10 != 10) << endl;
  cout << (0 < 10) << endl;
  cout << (10 < 0) << endl;
  cout << (10 > 0) << endl;
  cout << (0 > 10) << endl;
  cout << (0 <= 10) << endl;
  cout << (10 <= 0) << endl;
}
```

### Output:
```
1
0
1
0
1
0
1
0
1
0
```

```0``` equals False and ```1``` equals True.

## If statements
We can use the boolean comparisons for conditional decisions with if statements.

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  int num = 10;

  if (num == 10)
  {
    cout << "Do task" << endl;
  }

  num = 0;

  if (num == 10)
  {
    cout << "Do task" << endl;
  }
}
```

__Output:__
```
Do task
```

The second if statement does not get executed because the condition is false.
## Else statement
We can accomododate if statements with else statements which will execute when the if statement is false.

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  int num = 10;

  if (num == 10)
  {
    cout << "Do task" << endl;
  }

  else
  {
    cout << "Do different task" << endl;
  }

  num = 0;

    if (num == 10)
  {
    cout << "Do second task" << endl;
  }

  else
  {
    cout << "Do second different task" << endl;
  }
}
```

__Output:__
```
Do task
Do second different task
```
