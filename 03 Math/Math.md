# Math in C++

## Operators

In C++ we have the ability to do math operations. Here are the arithmetic operators we have available to us.

- ```+```: Addition
- ```-```: Subtraction
- ```*```: Multiplication
- ```/```: Division
- ```%```: Modulus (provides the division remainder)
- ```++```: increments a variable by 1
- ```--```: decrements a variable by 1

### Some examples of each operator:

### Addition:
```
#include<iostream>
using namespace std;

int main()
{
  int num1 = 6;
  int num2 = 3;
  int sum = 0;
  
  sum = num1 + num2;
  cout << sum << endl;
}
```

__Output:__

```9```

### Subtraction:
```
#include<iostream>
using namespace std;

int main()
{
  int num1 = 6;
  int num2 = 3;
  int diff = 0;
  
  diff = num1 - num2;
  cout << diff << endl;
}
```

__Output:__

```3```

### Multiplication:
```
#include<iostream>
using namespace std;

int main()
{
  int num1 = 6;
  int num2 = 3;
  int product = 0;
  
  product = num1 * num2;
  cout << product << endl;
}
```

__Output:__

```18```

### Division:
```
#include<iostream>
using namespace std;

int main()
{
  int num1 = 6;
  int num2 = 3;
  int dividend = 0;
  
  dividend = num1 / num2;
  cout << dividend << endl;
}
```

__Output:__

```2```

### Modulus:
```
#include<iostream>
using namespace std;

int main()
{
  int num1 = 6;
  int num2 = 3;
  int remainder = 0;
  
  remainder = num1 % num2;
  cout << remainder << endl;
  
  num1 = 14
  
  remainder = num1 % num2;
  cout << remainder << endl;
}
```

__Output:__

```
0
2
```

### Increment and Decrement
```
#include<iostream>
using namespace std;

int main()
{
  num = 0;
  num++;
  cout << num << endl;
  num++;
  cout << num << endl;
  num--;
  cout << num << endl;
  num--;
  cout << num << endl;
}
```

__Output:__

```
1
2
1
0
```

__OR__
```
#include<iostream>
using namespace std;

int main()
{
  num = 0;
  num=+1;
  cout << num << endl;
  num=+1;
  cout << num << endl;
  num-=1;
  cout << num << endl;
  num-=1;
  cout << num << endl;
}
```

__Output:__

```
1
2
1
0
```

## Math between data types
In C++ we have to be careful with calculations being done between ints and floats/doubles because the conversions can create loss of precision.
### Examples:
```
#include<iostream>
using namespace std;

int main()
{
  float num1 = 25;
  float num2 = 2;
  float f_sum = 0;
  int i_sum = 0;

  f_sum = num1 / num2;
  i_sum = num1 / num2;
  cout << f_sum << endl;
  cout << i_sum << endl;
}
```

__Output:__
```
12.5
12
```

As you can see with this example both ```num1``` and ```num2``` are floats and when the calculation is done with ```f_sum```, which is also a float, the solution is precise and equals 12.5. Although when the calculation is done with ```i_sum```, which is an int, the solution losses it's precision and the decimal gets dropped.

## Some useful math fuctions
C++ has a math library called ```<cmath>``` which includes more math operations and here are some of the useful noteworthy functions.

- ```pow(x,y)```: Calculates x to the power of y
- ```sqrt(x)```: Calculates the square root of x
- ```abs(x)```: Calculates the absolute value of x
- ```cbrt(x)```: Calculates the cube root of x

### Examples:
```
#include<iostream>
#include<cmath>
using namespace std;

int main()
{
  cout << pow(4,2) << endl;
  cout << sqrt(4) << endl;
  cout << abs(-4) << endl;
  cout << cbrt(8) << endl;
}
```

__Output:__
```
16
2
4
2
```
