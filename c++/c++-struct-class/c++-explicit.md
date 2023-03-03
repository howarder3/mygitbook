# C++ explicit

* 禁用 「=」 作為 constructor (copy-initialization)，只能 direct-initialization struct()
* 避免 10, "10" 分不清
* a = 10, a(10)&#x20;
  * explicit 禁用 a = 10
* a = "10", a("10")
* [https://shengyu7697.github.io/cpp-explicit/](https://shengyu7697.github.io/cpp-explicit/)
