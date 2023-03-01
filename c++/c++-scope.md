# C++ scope

```cpp
#include <iostream>

using namespace std;

int main(){

    int i = 0;
    cout << i << endl; // 0
    {
        i = 1;
        cout << i << endl; // 1
    }
    cout << i << endl; // 1   
    return 0;
}

```
