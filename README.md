# Это интерполятор для кривых терморезистора NTC3950

Впрочем, его можно использовать успешно и для других терморезисторов.

# Уравнение Стейнхарта-Харта

Уравнение [Стейнхарта-Харта](https://ru.wikipedia.org/wiki/Уравнение_Стейнхарта_—_Харта) ([Steinhart–Hart](https://en.wikipedia.org/wiki/Steinhart%E2%80%93Hart_equation))  математическая модель, описывающая сопротивление полупроводниковых терморезисторов с отрицательным температурным коэффициентом электрического сопротивления в зависимости от температуры.

Обычно, это уравнение описывают так:

![Уравнение Стейнахарта-Харта](fugures/st-hart.svg)

И обычно ограничиваются тремя точками при интерполяции этой кривой. Однако, точность при этом очень сильно страдает. 

Поэтому, стоит использовать библиотеку python [scipy](https://scipy.org/). Это значительно повышает точность полученных коэффициентов уравнения, что видно на пробном графике сравнения экспериментальной кривой и кривой полученной в результате интерполяции

![Графики апроксимированной функции и исходных данных термистора NTC3950](./figures/ntc3950.png)

# Запуск программы

В директории с программой запустить
```cmd
pip install -r /path/to/requirements.txt
```

Или в VSCode F1, (Ctrl+Shit+P), >Python: Create Environment

![Шаг 1](./fugures/inst_venv01.png)

> &gt; Python: Create Virtual Environment

![Шаг 2](./fugures/inst_venv02.png)

> &gt; Python: Select Interpreter

![Шаг 3](./fugures/inst_venv03.png)

> &gt; Using requirements.txt

![Шаг 4](./fugures/inst_venv04.png)

