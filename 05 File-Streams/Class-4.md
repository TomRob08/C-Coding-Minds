# Class 4
## File streams

C++ has a library that allows us to interact with files within our code which is: ```#include<fstream>```.

You may ask what's the difference between file streams and using files for input and output but the difference is files streams can interact with many files in our code and we have full control for when to use a file.

## Input file streams
### Exapmle:
```
#include<iostream>
#include<fstream>
using namespace std;

int main()
{
  string greeting;
  ifstream inputFile; //declares the varable to be an input file stream
  inputFile.open("inFile.txt");

  inputFile >> greeting;
  //OR getline(inputfile, greeting);
  cout << greeting << endl;
  return 0;
}
```

__infile.txt__
```
Hello
```

## Check if a file exists
```
if (!inputFile.is_open())
{
  cout << "Could not open the file" << endl;
  return 1; // This represents the code ended but an error occurred
}
```

### Exercises:
__1.__ Create these two files:

__animals.txt__
```
Dog
Cat
Rabbit
```

__phrases.txt__
```
Houston, we have a problem.
The quick brown fox jumps over the lazy dog.
Just keep swimming.
```

Write a program to check if both of these files exist and then print the content within the files.

## Output file streams
### Example:
```
#include<iostream>
#include<fstream>
using namespace std;

int main()
{
  string greeting = "Hello";
  ofstream outputFile; //declares the varable to be an output file stream
  outputFile.open("outFile.txt");

  outputFile << greeting;
  return 0;
}
```

### Exercises:
__1.__ Ask a user for their favorite animal and then add the animal to the animals.txt file.

__2.__ Ask a user what file they want to open. If the file exists then print it's contents but if it doesn't exist, allow the user to insert a sentence to a created file with the same name.

## String Manipulation
C++ has a library ```#include<string>``` that adds string related functions.

### String Concatenation:
```
#include <iostream>
#include <string>
using namespace std;
 
int main () 
{
  string firstName = "Jim ";
  string lastName = "Halpert";
  string fullName = firstName + lastName;
  //OR string fullName = firstName.append(lastName);
  cout << fullName << endl;
  return 0;
}
```

### Output:
```
Jim Halpert
```

### Convert strings to integers:
```
#include <iostream>
#include <string>
using namespace std;

int main()
{
  string numStr = "18";

  int num = stoi(numStr);

  cout << 2 + num << endl;
  return 0;
}
```

### Output:
```
20
```

### Convert integers to strings:
```
#include <iostream>
#include <string>
using namespace std;

int main()
{
  int num = 3;
  
  string three = to_string(num);
  cout << three << endl;
  
  return 0;
}
```

### String length:
Both ```length()``` and ```size()``` are viable ways of getting the length of a string.
```
#include <iostream>
#include <string>
using namespace std;

int main() 
{
  string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
  cout << "The length of the txt string is: " << txt.length() << endl;
  cout << "The length of the txt string is: " << txt.size() << endl;
  return 0;
}
```

### Output:
```
26
26
```

### Exercises:
__1.__ Concatinate these two strings: "Slam" "dunk".

__2.__ Convert "7" to an integer, add 3, then print the sum.

__3.__ Print the length of "Hippopotomonstrosesquippedaliophobia".

__4.__ Ask a user for a word and use an if statement to check if the word is greater than or equal to 8 letters. If it is less than 8 letters print "Your word needs to be at least 8 letters." and end the program. If the word is is greater or equal to 8 letters than ask the user for four numbers and concatinate the numbers to the end of the word. Print the result.
