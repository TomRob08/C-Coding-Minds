# Function Parameters

Data can be passed to functions and used in the function.

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
