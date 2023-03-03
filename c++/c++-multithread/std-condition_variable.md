# std::condition\_variable

* std::condition\_variable::wait
* [https://en.cppreference.com/w/cpp/thread/condition\_variable/wait](https://en.cppreference.com/w/cpp/thread/condition\_variable/wait)
  * 解除 mutex
  * 暫停 thread
  * 等待 notify 再次拿到 mutex, 繼續 thread
* condition\_variable wait
  * wait: unlock mutex, block thread
  * notify (喚醒): unblock thread
  * reaquire lock (next wait), wait exits
