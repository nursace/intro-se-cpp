# Lab 02 — Типы, I/O, cmath

1. `fx.cpp` — прочитать курс `rate` и сумму в USD, напечатать `USD <x> -> KGS <y>`.
2. `div.cpp` — прочитать `a` `b` (`int`), напечатать целочисленное и вещественное деление двумя строками.
3. `canteen.cpp` — блюдо (слово), цена, количество → строка вида `plov x2 = 180`.
4. `circle.cpp` — `const double PI`, радиус `r`. Площадь и длина окружности:

$$
S = \pi r^{2}, \quad C = 2\pi r
$$

Используйте `pow` или `r * r` из `<cmath>` / арифметики.

5. `distance2d.cpp` — точки `x1 y1 x2 y2`. Расстояние:

$$
d = \sqrt{(x_2 - x_1)^{2} + (y_2 - y_1)^{2}}
$$

API: `sqrt` или `hypot`.

6. `distance3d.cpp` — `x1 y1 z1 x2 y2 z2`:

$$
d = \sqrt{(x_2-x_1)^{2} + (y_2-y_1)^{2} + (z_2-z_1)^{2}}
$$

7. `heron.cpp` — стороны треугольника `a` `b` `c` (считать, что треугольник существует). Площадь по Герону:

$$
p = \frac{a + b + c}{2}, \quad S = \sqrt{p(p-a)(p-b)(p-c)}
$$

8. `cosine_law.cpp` — стороны `a` `b` и угол между ними `deg` (градусы). Третья сторона по теореме косинусов:

$$
c = \sqrt{a^{2} + b^{2} - 2ab\cos\alpha}, \quad \alpha = \deg \cdot \frac{\pi}{180}
$$

API: `cos`, `sqrt`, `pow` (или `*`).

9. `compound_month.cpp` — вклад `P`, годовая ставка `r` (доля), лет `t` (`int`). Капитализация ежемесячно:

$$
A = P\left(1 + \frac{r}{12}\right)^{12t}
$$

API: `pow`.

10. `quadratic.cpp` — `a` `b` `c` (`a ≠ 0`):

$$
D = b^{2} - 4ac, \quad x = \frac{-b \pm \sqrt{D}}{2a}
$$

Если $D \ge 0$ — напечатать оба корня; иначе `No real roots`. API: `sqrt`.

11. `trig.cpp` — угол `deg`:

$$
\alpha = \deg \cdot \frac{\pi}{180}
$$

Напечатать $\sin\alpha$ и $\cos\alpha$. API: `sin`, `cos`.

12. `projectile.cpp` — скорость `v`, угол `deg`, $g = 9.81$. Дальность броска:

$$
R = \frac{v^{2} \sin(2\alpha)}{g}, \quad \alpha = \deg \cdot \frac{\pi}{180}
$$

API: `sin`, `pow`.

13. `geo_mean.cpp` — три положительных числа `a` `b` `c`. Среднее геометрическое:

$$
G = \sqrt[3]{abc} = (abc)^{1/3}
$$

API: `pow` (например `pow(a * b * c, 1.0 / 3.0)`).

14. `stddev3.cpp` — три числа `x1 x2 x3`. Среднее и выборочное СКО (деление на $n-1 = 2$):

$$
\mu = \frac{x_1+x_2+x_3}{3}, \quad
s = \sqrt{\frac{(x_1-\mu)^{2}+(x_2-\mu)^{2}+(x_3-\mu)^{2}}{2}}
$$

API: `sqrt`, `pow` или `fabs` не обязателен.

15. `haversine.cpp` — две точки на сфере: широта/долгота в градусах `lat1 lon1 lat2 lon2`, радиус Земли `R = 6371` км. Упрощённо:

$$
\begin{aligned}
\varphi_i &= \mathrm{lat}_i \cdot \frac{\pi}{180},\quad
\lambda_i = \mathrm{lon}_i \cdot \frac{\pi}{180} \\
a &= \sin^{2}\frac{\Delta\varphi}{2} + \cos\varphi_1\cos\varphi_2\sin^{2}\frac{\Delta\lambda}{2} \\
d &= 2R \cdot \operatorname{atan2}\bigl(\sqrt{a},\, \sqrt{1-a}\bigr)
\end{aligned}
$$

API: `sin`, `cos`, `sqrt`, `atan2` (из `<cmath>`).

16. `body_bmi.cpp` — вес `kg`, рост `cm`:

$$
m = \frac{cm}{100}, \quad BMI = \frac{kg}{m^{2}}
$$

Напечатать BMI, `ceil(BMI)`, `floor(BMI)`.

17. `change.cpp` — одно `double x`: тремя строками `fabs`, `ceil`, `floor`.

`#include <cmath>`, `using namespace std;`
