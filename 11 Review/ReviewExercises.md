# Review Exercises

__1__. Using this code, complete the ```isPalindrome()``` function. A palindrome is any word that when reversed will be the same word. An example would be level, bob, racecar because if you revserse any of those words, they are still the same word. Some advice for writing the code would be to use the ```tolower()``` function.

Code:
```
#include <iostream>
#include <cctype>
using namespace std;

bool isPalindrome(string word)
{

}

int main() 
{
  string word = "";
  cout << "Please enter a word: " << endl;
  cin >> word;
  
  if(isPalindrome(word))
    cout << "This word is a palindrome" << endl;

  else
    cout << "This word is not a palindrome" << endl;
    
  return 0;
}
```

__2.__ Update the previous exercise so you can read in words from a file instad of user input. ```.eof()``` function might be helpful.

__3.__ Write a program that will count the number of words in a sentence.

__4.__ Write a program that decides if a given year was a leap year. Recent leap years have been 2008, 2012, 2016, and 2020.
