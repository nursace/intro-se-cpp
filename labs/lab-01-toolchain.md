# Lab 01 — Toolchain

1. `badge.cpp` — напечатать три строки: логин/фамилия, `Course: Intro SE (C++)`, `Build: OK`. Собрать с `-std=c++17 -Wall -Wextra`. Использовать `using namespace std;`.
2. `meet.cpp` — прочитать два имени и напечатать `Hello, <имя1> and <имя2>!`
3. Исправить `broken.cpp` (скопировать ниже), чтобы печатало `sum=15`. В комментарии перечислить найденные ошибки.

```cpp
#include <iostream>
using namespace std
int main( {
    int a = 7
    int b = 8;
    cout << "sum=" << a + b << "\n"
    return 0;
}
```

4. `warn_me.cpp` — намеренно получить warning (`-Wall -Wextra`), затем убрать его.
