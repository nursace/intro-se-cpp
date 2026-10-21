# Lab 11 — Каталог книг

1. Написать консольный каталог: команды `add`, `list`, `find`, `quit`.
2. Файлы: `book.h` / `book.cpp`, `library.h` / `library.cpp`, `main.cpp`, `REQUIREMENTS.md`.
3. `Library` хранит книги; `main` — только меню и ввод. В `.cpp` можно `using namespace std;`
4. Сборка: `g++ -std=c++17 -Wall -Wextra -o library_app main.cpp book.cpp library.cpp`
5. ≥3 автопроверки (`tests.cpp` или отдельный режим): add/list, find есть, find нет.
