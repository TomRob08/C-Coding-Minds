# Maps
A map is similar to a dictionary in Python.
 
 ## Map initialization
 ```
 #include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<int, string> mVar;
  
  return 0;
 }
 ```
 
We need to use ```#include <map>``` at the top the the code to use a map. When initializing a map we type ```map```, then state what the key and value types are in the map ```<int, string>```, and finally name the map variable. In the case of the example, our key is an ```int``` and the value is a ```string``` but the key and value can be any data type you'd like.

## Assigning values to maps
We assign values to maps by using the map key. Maps don't have a specific index for the keys so they can be anything but you should have it make sense to you and others.

### Example
```
#include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<int, string> mVar;

  mVar[1] = "one";
  mVar[2] = "two";
  mVar[3] = "three";
  
  return 0;
 }
```

## Accessing values in maps
We access values in maps by using the map's key.

### Example
```
#include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<int, string> mVar;

  mVar[1] = "one";
  mVar[2] = "two";
  mVar[3] = "three";

  cout << mVar[1] << endl;
  cout << mVar[2] << endl;
  cout << mVar[3] << endl;
  
  return 0;
}
```

### Output
```
one
two
three
```

__OR__ we can use ```.at(key)``` instead of brackets.

### Example
```
#include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<int, string> mVar;

  mVar[1] = "one";
  mVar[2] = "two";
  mVar[3] = "three";

  cout << mVar.at(1) << endl;
  cout << mVar.at(2) << endl;
  cout << mVar.at(3) << endl;

  return 0;
}
```

### Output
```
one
two
three
```

## Get map size
We can get the size of how many key:value pairs are in the map by using ```.size()```.

### Example
```
#include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<int, string> mVar;

  mVar[1] = "one";
  mVar[2] = "two";
  mVar[3] = "three";

  cout << mVar.size() << endl;

  return 0;
}
```

### Output
```
3
```

## Examples of other data type maps

### Char:String
```
#include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<char, string> mVar;

  mVar['a'] = "Apple";
  mVar['b'] = "Banana";
  mVar['c'] = "Coconut";

  cout << mVar['a'] << endl;
  cout << mVar['b'] << endl;
  cout << mVar['c'] << endl;

  return 0;
}
```

### Output
```
Apple
Banana
Coconut
```

### Float:Bool
```
#include <iostream>
#include <map>
using namespace std;

int main() 
{
  map<float, bool> mVar;

  mVar[1.8] = true;
  mVar[2.5] = false;
  mVar[3.0] = true;

  cout << mVar[1.8] << endl;
  cout << mVar[2.5] << endl;
  cout << mVar[3.0] << endl;

  return 0;
}
```

### Output
```
1
0
1
```
