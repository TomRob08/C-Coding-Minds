# Class 2

## Input
In C++ we use ```cin``` for gathering input from the terminal. It stands for "console in" so the console (console and terminal are the same) will input data to our program.

### Code Example
```
#include<iostream>
using namespace std;

int main()
{
  int num = 0;
  cout << "Please enter a number ";
  cin >> num; //This will set num to be the number a user entered
  cout << num << endl;
  
  return 0;
}
```

## Exercises
__1.__ Ask a user to enter two numbers and print the sum.

__2.__ Ask a user for their favorite color and then print it with your favorite color. The output should similar to this: ```Your favorite color is (user's color). Mine is (your color)```

## Input using text file
```cin``` can also use information from a text file as a form of input instead of user generated input.

### Text file
```
Dwight 37
```

### Code Example
```
#include<iostream>
using namespace std;

int main()
{
  string name;
  int age = 0;
  cout << "Please enter your name and age:\n";
  cin >> name >> age;

  cout << "Hello " << name << ". " << age << " is a great age.\n";
  
  return 0;
}
```

### Run the program in the terminal
```
$./main < inputFile.txt
```

### Output
```
Please enter your name and age:
Hello Dwight. 37 is a great age.
```

### Output response from program
Programs can be ran with the option to print ```cout``` messages to their own file instead of straight to the terminal.
```
$./main <inputFile.txt >outputFile.txt
```

### Compare and check if two files have the same information
```
$diff firstFile secondFile
```
If something gets printed then the two files have differences. If nothing happens then the two files are the same.

__OR__

```
$vimdiff firstFile secondFile
```
This will open a screen and show you the contents of both files. If a line if highlighted it means there is a difference. If nothing is highlighted it means both files are the same.

## Exercises
__1.__ Create text files for each of the previous exercises to achieve the same output.

__2.__ Ask a user for their favorite movie, it's release year, and it's iMDB rating. Use a text file for the input. (If the movie is more than one word then separate the words with an underscore)

# Getline

```getline()``` is a C++ function that uses ```cin``` to get the entire line from an input. The regular ```cin``` can only grab one word at a time but ```getline()``` can grab an entire sentence up until the newline character "\n". Files and terminal inputs have newline characters at the end of each line and ```getline()``` uses those to grab it's input data. ```getline()``` can only be used with strings.

## Code Example
```
#include<iostream>
using namespace std;

int main()
{
  string str = "";
  getline(cin, str);
  
  cout << str << endl;
  
  return 0;
}
```

### Input:
```Sometimes I’ll start a sentence and I don’t even know where it’s going. I just hope I find it along the way.```

### Output:
```Sometimes I’ll start a sentence and I don’t even know where it’s going. I just hope I find it along the way.```

## Exercises
__1.__ Do the second exercise from the previous set of exercises except this time don't put an underscore between the word for the movie title and make sure each input is on a separate line.

__2.__ Ask a user to enter their birthday (Month Day, Year), a song title, a quote they like, and their favorite restaurant. Store each input in a different variable.
