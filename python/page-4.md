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

