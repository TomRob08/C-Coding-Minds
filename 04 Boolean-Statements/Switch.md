# Switch Statement
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
