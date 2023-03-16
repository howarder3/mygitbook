# C++ const reference

* const reference
* [https://stackoverflow.com/questions/2627166/what-is-the-difference-between-a-const-reference-and-normal-parameter](https://stackoverflow.com/questions/2627166/what-is-the-difference-between-a-const-reference-and-normal-parameter)

```
// Pass by value
// copy object n, any change will change the copy n. (I.e. Origin n will not change.)
void f(int n){} 

// Pass by reference
// use original object n, any change will cause n change.
void f(int& n){}

// Constant reference
// no copy, n read only, can not change value n.
void f(const int& n){} 
```
