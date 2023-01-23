# Functions

Functions are blocks of code that can be called and ran. When a fuction is called in a program, the code block within the fuction is ran. The usefulness of a function is the ability to easily resuse code and have better code organization and management.

### Example:
```
#include <iostream>
using namespace std;

void hello() {
  cout << "Hello" << endl;
}

int main() {
  hello();
  return 0;
}
```

### Output:
```
Hello
```

A function can also be called multiple times.

### Example:
```
#include <iostream>
using namespace std;

void hello() {
  cout << "Hello" << endl;
}

int main() {
  hello();
  hello();
  hello();
  hello();
  return 0;
}
```

### Output:
```
Hello
Hello
Hello
Hello
```

## Function data types
As you can see in the example above, the ```hello()``` function has ```void``` in front which represents the data type that will be returned by the function when it is finished. In this case, ```void``` represents that nothing in the function will be returned as seen by only having ```cout << "Hello" << endl;``` in the function. ```int main()``` is also a function and it has ```int``` in the front so we use ```return 0``` when the function is finished. 

Functions can have any data type that a variable can have.

### Some examples of function data types:
```
#include <iostream>
using namespace std;

string words() {
  string phrase = "Slam dunk";
  return phrase;
}

float decimal() {
  return 3.9;
}

char letter() {
  return 'T';
}

bool TorF() {
  bool T = true;
  bool F = false;
  
  return T;
}

int main() {
  cout << words() << endl;
  cout << decimal() << endl;
  cout << letter() << endl;
  return 0;
}
```

### Output:
```
Slam dunk
3.9
T
```

The returned value or variable of a function is sent back to the exact location where the function is called and you have to either print it, set it to a variable, or use it in an operation otherwise nothing happens with the data returned.

## Function Declarations
A fuction can be declared at the top of a program and then the function block can be placed below the main function instead of being above it. This could help with readability and organization in some cases.

### Example:
```
#include<iostream>
using namespace std;

void printName();

int main()
{
  printName();
}

void printName()
{
  cout << "Sal" << endl;
}
```

### Output:
```
Sal
```

In the example, ```void printName();``` is placed at the top of the code and it declares a function called printName will be used somewhere in the program and in this case ```printName()``` is under ```main()```.

## Exercises:
__1.__ Write a function called countDown and have it print 10-0.

__2.__ Write a function called max that asks a user for two numbers, compares the two numbers and returns the larger number.

__3.__ Write another function called min that asks a user for two numbers, compares the two numbers and returns the smaller number. 

__4.__ Then organize the two min and max functions to be placed under ```main()```.
