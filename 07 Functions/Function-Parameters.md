# Function Parameters

Data can be passed to functions and be used in the function.

### Example:
```
#include<iostream>
using namespace std;

void printName(string name)
{
  cout << name << endl;
}

int main()
{
  printName("Terry");
}
```

### Output:
```
Terry
```

In the example above, ```name``` is called a parameter and ```Terry``` is the argument that is being passed into the function.

## Multiple parameters

Functions can also have multiple paramters that arguments will be passed into.

### Example:
```
#include<iostream>
using namespace std;

void printName(string name, int age)
{
  cout << name << endl;
  cout << age << endl;
}

int main()
{
  printName("Terry", 34);
}
```

### Output:
```
Terry
34
```

## Pass by Reference
Pass by reference is when data is shared to a function from the area where the function was called. The data in the original place is changed whenever it is also changed in the function.

### Example:
```
#include<iostream>
using namespace std;

void changeName(string& name)
{
  name = "Jill";
}

int main()
{
  string fname = "Terry";
  cout << fname << endl;
  
  changeName(fname);
  
  cout << fname << endl;
}
```

### Output
```
Terry
Jill
```

As seen in the fuction delaration, a ```&``` denotes that a parameter will be a pass by reference parameter and that sign can be used right next to the data type or variable name such as: ```string& name``` or ```string &name```.

## Exercises
__1.__ Write a function that has two parmeters for numbers and returns the sum of the numbers.

__2.__ Write a function that uses pass by reference to swap two numbers.

__3.__ Using the code below write a function named ```movieRating``` that uses pass by reference for the first parameter and the second parameter is regular. The argument entered into the first parameter will be ```rating```, the second argument will be ```movie```. Inside of the fuction ask the user what they would rate the provided movie between 1 and 5 and average their rating with the movie's rating.
```
#include<iostream>
using namespace std;

int main()
{
  float rating; // assign this variable a number between 1 - 5
  string movie; // assign this variable your favorite movie
  
  movieRating(rating, movie);
  cout << rating << endl;
  
  return 0;
}
```
