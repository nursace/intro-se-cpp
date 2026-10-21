# Lab 02 — Типы, I/O, cmath

1. `fx.cpp` — прочитать курс `rate` и сумму в USD, напечатать `USD <x> -> KGS <y>`.
2. `div.cpp` — прочитать `a` `b` (`int`), напечатать целочисленное и вещественное деление двумя строками.
3. `canteen.cpp` — блюдо (слово), цена, количество → строка вида `plov x2 = 180`.
4. `circle.cpp` — `const double PI`, радиус `r`: площадь \(S = \pi r^{2}\) (`pow` или `r*r`) и длина \(C = 2\pi r\).
5. `distance.cpp` — точки `x1 y1 x2 y2`: \(d = \sqrt{(x_2-x_1)^2+(y_2-y_1)^2}\) через `sqrt` (или `hypot`).
6. `hypot3.cpp` — катеты `a` `b` `c` в 3D: \(d = \sqrt{a^{2}+b^{2}+c^{2}}\) (`sqrt` + `pow`, либо `hypot(hypot(a,b), c)`).
7. `compound.cpp` — вклад: сумма `P`, ставка `r` (доля, напр. `0.05`), лет `n` (`int`): \(A = P(1+r)^{n}\) через `pow`; напечатать `A`.
8. `quadratic.cpp` — коэффициенты `a` `b` `c` (`a ≠ 0`): дискриминант \(D = b^{2}-4ac\); если \(D \ge 0\), корни \(x = \frac{-b \pm \sqrt{D}}{2a}\) (`sqrt`, `fabs` не обязателен); иначе `No real roots`.
9. `trig.cpp` — угол `deg` в градусах: перевести в радианы \(\alpha = \deg \cdot \pi / 180\), напечатать `sin(α)` и `cos(α)`.
10. `body_bmi.cpp` — вес `kg`, рост `cm`: \(BMI = kg / (m)^{2}\), где \(m = cm/100\); напечатать BMI и `ceil(BMI)`, `floor(BMI)`.
11. `change.cpp` — одно `double x`: тремя строками `fabs`, `ceil`, `floor`.

`#include <cmath>`, `using namespace std;`
