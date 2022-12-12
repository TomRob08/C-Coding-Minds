# Homework 5
## User login interface
Stark Industries has come to you to create a user login interface for their offices. They have files for all of their employees on record containing the user account number and password and the file is named the employees name. Here are some of the files.

[Kelly.txt](https://github.com/TomRob08/C-Coding-Minds/files/10203706/Kelly.txt)
```
59762
#CocoTheChocolateLab84
```

[Paul.txt](https://github.com/TomRob08/C-Coding-Minds/files/10203707/Paul.txt)
```
35876
0toHero*
```

[Tim.txt](https://github.com/TomRob08/C-Coding-Minds/files/10203708/Tim.txt)
```
37228
tim$cool4sure
```

Use these files to check if what a user enters is correct.

### Exapmle output (Places with // is user input):
```
Hello, welcome to Stark Industries.
What is your name?
//Tim
Please enter your account number:
//37228
Please enter your password:
//tim$cool4sure
Thank you Tim for logging in.
```

You should also prevent people from continuing to log in after 3 incorrect tries and if their name isn't in the system.

### Example output with incorrect tries (Places with // is user input):
```
Hello, welcome to Stark Industries.
What is your name?
//Tim
Please enter your account number:
//11111
Sorry, incorrect number. Try again.
///22222
Sorry, incorrect number. Try again.
///33333
You have exhausted your tries.
```

__OR__
```
Hello, welcome to Stark Industries.
What is your name?
//Tim
Please enter your account number:
//37228
Please enter your password:
//Hello
Sorry, incorrect password. Try again.
///World
Sorry, incorrect password. Try again.
//Light
You have exhausted your tries.
```

__OR__
```
Hello, welcome to Stark Industries.
What is your name?
//Jenny
That name is not in our system.
```

## Concepts used for this assignment:
- String manipulation
- fstream file input
- while loops
- bool variable
- if statements
