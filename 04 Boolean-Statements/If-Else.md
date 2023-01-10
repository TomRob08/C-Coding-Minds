# If-Else

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

## Else if statement
An Else if statement allows for more precise conditions since it has more granularity.

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  int num = 15;

  if(num < 10)
  {
    cout << "num is less than 10\n";
  }

  else if(num < 20)
  {
    cout << "num is less than 20\n";
  }

  else
  {
    cout << "num is greater than to equal to 20\n";
  }
}
```

__Output:__
```
num is less than 20
```

## Side note/Fun fact
In C++, if and else statements do not require brackets if the code inside is only a single line of code. If we look at the previous example, we can change it to not have brackets.
```
#include<iostream>
using namespace std;

int main()
{
  int num = 15;

  if(num < 10)
    cout << "num is less than 10\n";

  else if(num < 20)
    cout << "num is less than 20\n";

  else
    cout << "num is greater than to equal to 20\n";
}
```

__Output:__
```
num is less than 20
```

### Invalid Code
```
#include<iostream>
using namespace std;

int main()
{
  int num = 1;

  if(num < 10)
    cout << "num is less than 10\n";
    cout << "Hello\n";

  else if(num < 20)
    cout << "num is less than 20\n";

  else
    cout << "num is greater than to equal to 20\n";
}
```
Since the if statement had two lines of code, the program will not compile.
