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

## Exercises:
__1.__ Write a function called countDown and have it print 10-0.

__2.__ 
