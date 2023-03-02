---
description: 內建前身
---

# 內建 venv (前身 virtualenv)

要先想辦法安裝 python 你要的版本至 base



開啟 venv

```
# 依照你的版本
python -m venv <your_env_path>
python3 -m venv <your_env_path>
# 甚至可能是
python3.10 -m venv <your_env_path>
```

source activate venv python not working

```
# 確認 softlink 是否正確 (可能是 /usr/bin/python3.9)
ll ./myenvs/python39/lib/python3.9
```

* [https://ithelp.ithome.com.tw/articles/10199980](https://ithelp.ithome.com.tw/articles/10199980)
* python 3.10 venv
* [https://docs.python.org/zh-tw/3.10/library/venv.html](https://docs.python.org/zh-tw/3.10/library/venv.html)
* python venv
* [https://ithelp.ithome.com.tw/articles/10199980](https://ithelp.ithome.com.tw/articles/10199980)
* venv stopped working
* [https://stackoverflow.com/questions/58117467/python-venv-not-creating-virtual-environment](https://stackoverflow.com/questions/58117467/python-venv-not-creating-virtual-environment)
* python3.9 venv returned non-zero exit status 1.
* [https://stackoverflow.com/questions/24123150/pyvenv-3-4-returned-non-zero-exit-status-1](https://stackoverflow.com/questions/24123150/pyvenv-3-4-returned-non-zero-exit-status-1)
* Command '\[m', 'ensurepip', '--upgrade', '--default-pip']' returned non-zero exit status 1.
* [https://stackoverflow.com/questions/24123150/pyvenv-3-4-returned-non-zero-exit-status-1](https://stackoverflow.com/questions/24123150/pyvenv-3-4-returned-non-zero-exit-status-1)
* source activate venv alias not change
* [https://superuser.com/questions/1281343/activate-virtualenv-using-alias](https://superuser.com/questions/1281343/activate-virtualenv-using-alias)

