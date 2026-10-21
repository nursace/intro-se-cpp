# Lab 10 — Отладка и тесты

1. Исправить `buggy_average.cpp` (ниже); в комментарии перечислить баги.

```cpp
#include <iostream>
#include <vector>
using namespace std;

double average(const vector<int>& v) {
    int sum = 0;
    for (int i = 0; i <= v.size(); ++i) {
        sum += v[i];
    }
    return sum / v.size();
}

int main() {
    vector<int> v{1, 2, 3, 4};
    cout << average(v) << "\n";
}
```

2. `clamp_test.cpp` — `clamp` + ≥5 `assert` (границы, середина).
3. `grade_test.cpp` — `letter_grade` + счётчики `passed`/`failed` (≥6 кейсов); при ошибках `return ≠ 0`.
4. Зафиксировать поведение `average` на пустом векторе и покрыть тестом.
5. `broken_max.cpp` — сначала сломанный `max_of` + падающие тесты, затем исправить.

`using namespace std;`
