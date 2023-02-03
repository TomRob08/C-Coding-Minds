# Arrays

## Initialization of arrays

### Empty array
```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5];
  
  return 0;
}
```

```string``` is the data type of the array. All values inside of an array must be the same datatype that is specified. Arrays can be any datatype we have talked about before.

```strArray``` is the name if the array.

```[5]``` is the size of the array. Arrays must be assigned a size when initialized because they are static. Arrays also cannot increase in size after initialization

### Array with values
```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5] = {"The", "dog", "is", "very", "fast"};
  //OR
  string strArray[] = {"The", "dog", "is", "very", "fast"};
  
  return 0;
```

Array can be initialized with values if there is an equal sign on the right and then the array values inside curly brackets ```{}```. Arrays don't need to have their size declared if it is initialized with values because the array knows it's size based on how many values are in the curly brackets.

## Accessing values in an array

Arrays have an index that specifies value positions. The index counts starting at 0 and goes up by 1 to the max size of the array.

### Get value at index
```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5] = {"The", "dog", "is", "very", "fast"};

  cout << "1st value of array: " << strArray[0] << endl;
  cout << "2nd value of array: " << strArray[1] << endl;
  cout << "3rd value of array: " << strArray[2] << endl;
  cout << "4th value of array: " << strArray[3] << endl;
  cout << "5th value of array: " << strArray[4] << endl;
  
  return 0;
}
```

__Output__
```
1st value of array: The
2nd value of array: dog
3rd value of array: is
4th value of array: very
5th value of array: fast
```

### Update value at index
Let's start with the empty array and fill it with values, then update the second value to "cat".

```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5];

  strArray[0] = "The";
  strArray[1] = "dog";
  strArray[2] = "is";
  strArray[3] = "very";
  strArray[4] = "fast";

  cout << "1st value of array: " << strArray[0] << endl;
  cout << "2nd value of array: " << strArray[1] << endl;
  cout << "3rd value of array: " << strArray[2] << endl;
  cout << "4th value of array: " << strArray[3] << endl;
  cout << "5th value of array: " << strArray[4] << endl;

  strArray[1] = "cat";

  cout << "2nd value of updated array: " << strArray[1] << endl;
  
  return 0;
}
```

__Output___
```
1st value of array: The
2nd value of array: dog
3rd value of array: is
4th value of array: very
5th value of array: fast
2nd value of updated array: cat
```

### Values cannot be added to an array
If we use the same array we have been using and try adding a value at index 5, it will give an error.
```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5];

  strArray[0] = "The";
  strArray[1] = "dog";
  strArray[2] = "is";
  strArray[3] = "very";
  strArray[4] = "fast";
  strArray[5] = "outside";

return 0;
}
```

__Output__
```
signal: segmentation fault (core dumped)
```
Segmentation fault means we are trying to access something outside of the memory available for the array.


## Looping through an array

### For loop
```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5] = {"The", "dog", "is", "very", "fast"};

  for(int i = 0; i < 5; i++)
  {
    cout << strArray[i] << endl;
  }
}
```

__Output__
```
The
dog
is
very
fast
```

### For-each loop
Similar to ```for i in list``` in Python

```
#include <iostream>
using namespace std;

int main() 
{
  string strArray[5] = {"The", "dog", "is", "very", "fast"};

  for (string i : strArray)
  {
    cout << i << endl;
  }
}
```

__Output__
```
The
dog
is
very
fast
```
