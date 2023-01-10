# Class 1

## Our first C++ program
```
#include<iostream>
using namespace std;
  
int main()
{
  cout << "Hello world" << endl;
  return 0;
}
```

### Here is an explaination of each part of the program:
```#include<iostream>```: Allows the program to output data to the terminal. It also allows your program to have input from the terminal. Hence the “io” in “iostream” and the stream refers to the thought of data flowing in and out like a river.

```using namespace std;```: Std is a library also known as the standard library and we use it to inform the program there will be code that uses tools from the standard library. ```cout``` and ```endl``` are examples of some of the tools from the std library.

```int main()```: This is called a function in which we will learn about functions later but for now it is where we will type our code within the brackets.

```cout```: Outputs data to the terminal. If ```using namespace std;``` wasn't in this program we would type ```std::cout```.

```endl```: Tells the terminal to include a newline after printing. If ```using namespace std;``` wasn't in this program we would type ```std::endl```.

```;```: C++ requires semicolons to be placed at the end of code statements.

```return 0;```: This informs the compiler our code has completed without any errors.

## Variables
Variables are used in programming to store data. Imagine storing an item inside of a box.

## Data types
Data types define what can be stored in a variable.

```int```: Integers are whole numbers. Some examples would be: 5, 10, -5, -10.

```float```: Floats are decimal numbers. Some examples would be: 6.3, 2.0, -8.9, -5.1.

```string```: Strings are anything within double quotation marks. Some examples would be: "Hello", "eight", "8", "I like programming".

```char```: Chars are anything within single quotations marks. They only store single characters.

```bool```: Booleans store True and False.

## Example of Variables being used in a program
```
#include<iostream>
using namespace std;
  
int main()
{
  int num = 7;
  float decimal = 9.6;
  string str = "Hello";
  
  cout << num << " " << decimal << " " << str << endl;
  
  return 0;
}
```

### Output of program:
```7 9.6 Hello```
