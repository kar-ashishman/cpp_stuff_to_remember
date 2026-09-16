> 01: std::fill()
```
// The following code prints
// 5
// 5
// 5
#include<iostream>
#include<array.h>
int main() {
  std::array <int, 3>arr;
  std::fill(std::begin(arr), std::end(arr), 5);
  for(auto& element: arr) std::cout << element << std::endl;
}
```
<br>

> 02: Different return type declaration

Used for lambda functions and better visibility of various function declaration
```
auto testFunction(int arg, int args*) -> float;
```
<br>

> 03: Type Information `typeid`

Get the type of a variable
```
// Following program prints i i which stands for integer
#include <iostream>
#include<typeinfo>
int main() {
  int x = 10;
  int& y = x;
  std::cout << typeid(x).name() << " " << typeid(y).name();
}
```

> 04: Always make arguments `const`

Do this wherever it is possible, such that functions <br>
will not be able to accidentally change the data that belongs to their parent functions


