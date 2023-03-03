# call by value, call by address, call by reference

###

* call by value, call by address, call by reference 差別在哪?
* [https://wayne265265.pixnet.net/blog/post/112556555-【教學】call-by-value%2C-call-by-address%2C-call-by-referenc](https://wayne265265.pixnet.net/blog/post/112556555-%E3%80%90%E6%95%99%E5%AD%B8%E3%80%91call-by-value%2C-call-by-address%2C-call-by-referenc)
* #### Call by value
*   #### 結果 :

    \==a的值仍然是1, 而a的值複製到了b的記憶體區域, 所以b現在的值也是1。==

    注意事項 :

    當你利用call by value的方法去傳值時因為a與b的記憶體是分開的，所以不會互相干擾，但也需要兩個記憶體去儲存他們，這時候請仔細思考是否有使用call by value的必要，如果之後在較大型的程式運行時，==若使用太多call by value而使用結束後沒有刪除掉未使用的記憶體空間，可能會導致記憶體不足而程式崩潰==，切記切記!

```
int main() {
    int a = 1 ;
    int b = a ; //將a的值複製到b的新記憶體區域

    return 0;
}
```

* #### Call by address (Call by pointer)
*   在這個例子中，==使用了一個swap function，它的功能是將a和b傳入的address進行交換==，之後在main裡面利用&符號傳入address，然後執行一遍就可以發現，交換前a的值為1，b的值為0，交換後a的記憶體空間和b交換，所以各自代表的值也變成了0和1。

    當你使用call by address時，經常會使用到pointer，想當年當接觸C, C++的我對於pointer(指標)也是一知半解，符號\*和&的用法除了知道理論外動手實際去做一遍才能熟能生巧，之後介紹一篇pointer的教學吧

```
void swap(int *address_a, int *address_b) {
    int temp = *address_a ; 
    *address_a = *address_b;
    *address_b = temp;
}

int main() {

    int a = 1;
    int b = 0;

   cout<< a << " " << b << endl; // 1 0

    swap(&a, &b); // 傳入a, b的address進行交換

    cout<< a << " " << b << endl; // 0 1

    return 0;
}
```

* Call by reference
* 看起來是不是和call by address很像呢，其實他也是==利用pointer的方法實作，只是更簡潔==，但這個方法只能在C++上使用，所以寫C的朋友們將就點使用call by address吧 !

```
void swap(int &address_a, int &address_b) {
    int temp = address_a ; 
    address_a = address_b;
    address_b = temp;
}

int main() {

    int a = 1;
    int b = 0;

   cout<< a << " " << b << endl; // 1 0

    swap(a, b); // 傳入a, b的address進行交換

    cout<< a << " " << b << endl; // 0 1

    return 0;
}

```
