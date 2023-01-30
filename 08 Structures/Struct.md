# Structures

Structures or Structs are ways of storing related data under one object with many member variables. Member variables can be different data types.

### Exapmle:
```
#include <iostream>
using namespace std;

// Creating the structure
struct structure_name
{
  int num; //member var1
  string str; //member var2
  float decimal; //member var3
};

int main() 
{
  // Single line intialization
  structure_name var1 = {5, "Hello", 3.14};

  // Accessing var1 variables
  cout << "Var1 num: " << var1.num << endl;
  cout << "Var1 str: " << var1.str << endl;
  cout << "Var1 decimal: " << var1.decimal << endl;

  // Multi line intialization
  structure_name var2;
  var2.num = 8;
  var2.str = "World";
  var2.decimal = 7.3;

  // Accessing var2 variables
  cout << "Var2 num: " << var2.num << endl;
  cout << "Var2 str: " << var2.str << endl;
  cout << "Var2 decimal: " << var2.decimal << endl;

  return 0;
}
```

### Output:
```
Var1 num: 5
Var1 str: Hello
Var1 decimal: 3.14
Var2 num: 8
Var2 str: World
Var2 decimal: 7.3
```

In the example above we have a structure named ```structure_name``` that has three member variables called ```num```, ```str```, and ```decimal``` and it is created above the ```main()``` function but structures can also be created within the ```main()``` function. The variables ```var1``` and ```var2``` are created as the struct variables and they contain the values for each member variable.

## Exercises
__1.__ Use this struct named ```car``` and create one struct variable called ```car1```. Initialize the struct variable and assign values, 2008 Toyota Prius, for the member variables. Print the values.
```
struct car
{
  int year;
  string make;
  string model;
}
```

__2.__ Create a struct named ```Box``` with ```height```, ```width```, and ```length``` as it's member variables. Initialize a struct variable and assign values for each member variable. Then print the volume of the box.

__3.__ Create a struct named ```basketball_player```. Then go to <https://www.nba.com/players>, find your favorite player, and create member variables for some of the stats listed. Initialize a struct variable with the name of the player and assign values for that players stats.
