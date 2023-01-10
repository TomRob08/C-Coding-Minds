# Boolean Comparisons
### Comparison Operators:
- ```==```: Equal to. Checks to see if the two values are the same.
- ```!=```: Not equal
- ```>```: Greater than
- ```<```: Less than
- ```>=```: Greater than or equal to
- ```<=```: Less than or equal to

### Examples:
```
#include<iostream>
using namespace std;

int main()
{
  cout << (10 == 10) << endl;
  cout << (10 == 0) << endl;
  cout << (0 != 10) << endl;
  cout << (10 != 10) << endl;
  cout << (0 < 10) << endl;
  cout << (10 < 0) << endl;
  cout << (10 > 0) << endl;
  cout << (0 > 10) << endl;
  cout << (0 <= 10) << endl;
  cout << (10 <= 0) << endl;
}
```

### Output:
```
1
0
1
0
1
0
1
0
1
0
```

```0``` equals False and ```1``` equals True.
