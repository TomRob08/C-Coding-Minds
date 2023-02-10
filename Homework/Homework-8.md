# Homework 8
Your friend wants to make a program that calculates the price they will pay at the gas station based on what octane is choosen and how many gallons they want but it seems to not be working. There are a total of 5 bugs in this program that are preventing it from running correctly. Please help find the bugs in the program. There is an example of the desired output below the code. 

```
#include <ostream>
#include <map>
using namespace std; 

float getPrice(int octane, float gallons);

int main() 
{ 
  int octane = 0;
  float gallons = 0;
  float price;

  cout << "Welcome to the gas station. Would you like 87, 89, or 91 Octane?" << endl;
  cin >> octane;

  while(true)
  {
    if(octane == 87 && octane == 89 && octane == 91)
    {
      cout << "How many gallons do you want?" << endl;
      cin >> gallons;

      price = getPrice(octane, gallons);

      cout << "Your price for gas will be: $" << price << endl;
      return 0;
    }

    else
    {
      cout << "Incorrect octane" << endl;
      cout << "Would you like 87, 89, or 91 Octane?" << endl;
    }
  }
}

float getPrince(int octane, float gallons)
{
  map<int, int> prices;
  prices[87] = 3.99;
  prices[89] = 4.29;
  prices[91] = 4.39;

  return prices[octane] * gallons;
}
```

### Desired output example
```
Welcome to the gas station. Would you like 87, 89, or 91 Octane?
87
How many gallons do you want?
13
Your price for gas will be: $51.87
```
