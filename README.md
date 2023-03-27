# Markdown cheatsheet
<!-- Комментарий -->

# Заголовок первого уровня
## Заголовок второго уровня
### Заголовок третьего уровня

```
# Заголовок первого уровня
## Заголовок второго уровня
### Заголовок третьего уровня
```

# Форматирование

*Текст курсивом*  
_Текст курсивом_
```
*Текст курсивом*  
_Текст курсивом_
```

**Текст жирным**  
__Текст жирным__
```
**Текст жирным**  
__Текст жирным__
```

***Жирный курсив***
___Жирный курсив___
```
***Жирный курсив***
___Жирный курсив___
```

_Можно **комбинировать** форматирование_
```
_Можно **комбинировать** форматирование_
```

~~Зачёркнутый текст~~
```
~~Зачёркнутый текст~~
```

<ins>Подчёркнутый</ins>
```
<ins>Подчёркнутый</ins>
```

<sub>Подстрочный</sub>Текст в строке<sup>Надстрочный</sup>
```
<sub>Подстрочный</sub>Текст в строке<sup>Надстрочный</sup>
```

<samp>Моноширинный текст</samp>
```
<samp>Моноширинный текст</samp>
```


# Списки

## Ненумерируемые

* Элемент 1
* Элемент 2
  * Элемент 2.1
  * Элемент 2.2
    * Элемент 2.2.1
  * Элемент 2.3
* Элемент 3

```
* Элемент 1
* Элемент 2
  * Элемент 2.1
  * Элемент 2.2
    * Элемент 2.2.1
  * Элемент 2.3
* Элемент 3
```

Вместо `*` можно использовать `+` или `-`.

## Нумерируемые

1. Элемент 1
4. Элемент 2
   1. Элемент 2.1
   7. Элемент 2.2
      1. Элемент 2.2.1
   4. Элемент 2.3
0. Элемент 3

```
1. Элемент 1
4. Элемент 2
   1. Элемент 2.1
   7. Элемент 2.2
      1. Элемент 2.2.1
   4. Элемент 2.3
0. Элемент 3
```
Порядок цифр не важен, но первая обязательно 1.

## Список задач

- [x] Выполненная задача
- [ ] Невыполненная задача

```
- [x] Выполненная задача
- [ ] Невыполненная задача
```

# Изображения

![fortran logo]
```
![fortran logo]

[fortran logo]: https://fortran-lang.org/ru/_static/fortran-logo-256x256.png "Фортран"
```

Также можно без выноса ссылки: `![Альтернативный текст](Ссылка)`.


### Более хитрый способ с настройкой размера

[<img src="https://fortran-lang.org/ru/_static/fortran-logo-256x256.png" width="100"/>][fortran logo]

[fortran logo]: https://fortran-lang.org/ru/_static/fortran-logo-256x256.png "Фортран"

```
[<img src="..." width="100"/>][fortran logo]

[fortran logo]: ... "Фортран"
```

# Ссылки

Ссылка на сайт [Фортрана](https://fortran-lang.org/ru/index#).
Вынесенная ссылка на сайт [Фортрана][fortran link].

[fortran link]: https://fortran-lang.org/ru/index#

Также ссылку можно вставить целиком https://fortran-lang.org/ru/index#

```
Ссылка на сайт [Фортрана](...).
Вынесенная ссылка на сайт [Фортрана][fortran link].

[fortran link]: https://fortran-lang.org/ru/index#
```

# Цитаты

> Первый уровень цитирования
>> Второй уровень цитирования
> 
> Первый уровень цитирования

```
> Первый уровень цитирования
>> Второй уровень цитирования
> 
> Первый уровень цитирования
```

# Таблицы

| Заголовок слева      | Заголовок выровненный | Заголовок справа     |
| -------------------- | :-------------------: | -------------------- |
| Содержимое таблицы 1 | Содержимое таблицы 2  | Содержимое таблицы 3 |

```
| Заголовок слева      | Заголовок выровненный | Заголовок справа     |
| -------------------- | :-------------------: | -------------------- |
| Содержимое таблицы 1 | Содержимое таблицы 2  | Содержимое таблицы 3 |
```

Автоформатирование в VSCode: <kbd>Option</kbd> + <kbd>Shift</kbd> + <kbd>F</kbd>

# Фрагменты кода

```fortran
call MPI_INIT(err)
call MPI_COMM_SIZE(MPI_COMM_WORLD, nprocs, err)
call MPI_COMM_RANK(MPI_COMM_WORLD, myID, err)
```

````
```fortran
call MPI_INIT(err)
call MPI_COMM_SIZE(MPI_COMM_WORLD, nprocs, err)
call MPI_COMM_RANK(MPI_COMM_WORLD, myID, err)
```
````

## Inline код

Любая прикладная MPI-программа (приложение) должна начинаться с вызова функции инициализации MPI — `MPI_INIT(err)`.

```
Любая прикладная MPI-программа (приложение) должна начинаться с вызова функции инициализации MPI — `MPI_INIT(err)`.
```

# Горизонтальная черта

Горизонтальная черта через `***`
***
Горизонтальная черта через `___`

---

# Emoji

:sunny: :+1: :classical_building:

```
:sunny: :+1: :classical_building:
```

[Emoji picker](https://github-emoji-picker.rickstaa.dev)

# Комбинации клавиш

<kbd>Command</kbd> + <kbd>S</kbd>
```
<kbd>Command</kbd> + <kbd>S</kbd>
```

# Математические выражения

Формула в строке: $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$

Формула на всю ширину:
```math
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
```

````
Формула в строке: $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$

Формула на всю ширину:
```math
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
```
````

[Подробнее про LaTeX](https://en.wikibooks.org/wiki/LaTeX/Mathematics)

[MathJax basic tutorial and quick reference](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference/22395#22395)

# Спойлеры

<details><summary>Подробнее</summary>
<p>
Текст под спойлером
</p>
</details>

```html
<details><summary>Подробнее</summary>
<p>
Текст под спойлером
</p>
</details>
```

# Диаграммы

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

````
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

[Подробнее про Mermaid](https://mermaid.js.org)

# Ссылки на источники

[Markdown-Cheatsheet](https://github.com/lifeparticle/Markdown-Cheatsheet)

[Markdown Support for Visual Studio Code](https://github.com/yzhang-gh/vscode-markdown)

[Writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/)

