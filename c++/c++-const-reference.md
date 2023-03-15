# C++ const reference

* const reference
* [https://stackoverflow.com/questions/2627166/what-is-the-difference-between-a-const-reference-and-normal-parameter](https://stackoverflow.com/questions/2627166/what-is-the-difference-between-a-const-reference-and-normal-parameter)

```
void f(int n){} // copy object n, any change will change the copy n. (I.e. Origin n will not change.)
void f(int& n){} // use original object n, any change will cause n change.
void f(const int& n){} // no copy, n read only, can not change value n.
```
