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


## Switch Statement
C++ also has another conditional called a switch. A switch statement allows a variable to be tested for equality against a list of cases and the variable being switched on is checked for each case.

### General format of Switch statement
```
switch(variable) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

### Example:
```
#include<iostream>
using namespace std;

int main()
{
  //time is in 24-hour clock format
  int time = 1;

  switch(time)
  {
    case 8:
      cout << "Breakfast\n";
      break;

    case 13:
      cout << "Lunch\n";
      break;

    case 18:
      cout << "Dinner\n";
      break;

    default:
      cout << "Not eating time\n";
      break;
  }
}
```

### Exercises
__1.__  Create a switch statement for grades recieved by students. Print responces for each of the following grades; 
- A: Excellent 
- B: Good job
- C: Average
- D: Could have done better
- F: Good luck next time
- Any other letter: Invalid grade

__2.__ Create a switch statement for days of the week. We will use numbers to correspond with each day of the week from 0-6 which will match up with Sunday-Saturday. If a number is not within 0-6 then print "Invalid day".

__3.__ Bonus: Create the first part of a rock, paper, scissors game using a switch statement. Ask a user to choose 1, 2, or 3 and use a switch statement to print rock for 1, paper for 2, and scissors for 3.
