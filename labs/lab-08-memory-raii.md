# Lab 08 — Память и RAII

1. `raw_sum.cpp` — `n`, `new int[n]`, сумма, `delete[]`; комментарий про утечку.
2. `vector_sum.cpp` — то же через `vector` без `new`/`delete`.
3. `unique_counter.cpp` — `Counter` через `make_unique`, несколько `inc`, печать значения.
4. `grade_buffer.cpp` — класс с `vector<int>` внутри: размер, `set`, `get`, `size`.
5. `fixed_leak.cpp` — переписать API `make_ones` так, чтобы возвращать `vector<int>` (без забываемого `delete[]`).

`using namespace std;` Сырой `new` — только в задаче 1.
