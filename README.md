# Pybind11 の使用方法

- Ubuntu コンテナ内

```bash
clang++ -O3 -Wall -shared -std=c++14 -fPIC `python3.10 -m pybind11 --includes` myadd.cpp -o myadd`python3.10-config --extension-suffix` -I /usr/include/python3.10
```