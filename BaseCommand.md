<!--Заголовки-->
# Людмила
## Людмила
### Людмила
#### Людмила
##### Людмила
###### Людмила

Людмила еще 1

===

<!--Выделение текста-->
*курсив*
**жирный**
***жирный курсив***
<!--Выделение блоков-->
___

---
<!--зачеркнутый текст-->
~~**text**~~

<!--Абзацы-->


<!--Списки, зачеркивание-->

<!--Не нумерованнные списки людым из 3 способов-->
+ Англия
+ Италия
+ Германия

* США
* Мексика
* Бразилия

- Греция
- Италия
- Испания

<!--Нумерованные спискиб если начинаем с 1 то все последующая номерация попорядкуб чтобы мы не писали-->
1. Англия
2. Италия
3. Германия
10.
1. Греция
2. Италия
18. Испания
<!--Если на чинаем с другой цифрыб например 50, то и номерация будет продолжаться с 50 и далее попорядку-->
50. США
12. Мексика
25. Бразилия
51.
52.

<!--Вложенные списки-->
1. Англия
    * Бигбег
    * Мини купер
    * Автобус
2. Италия
3. Франция


<!--Ссылки-->
[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)
<!--если хотим подсказку при подсвечивании ссылки-->
[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/ "Мой линкедин")

Здравствуйтеб это мой линкедин: <[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)>


<!--Цитаты-->
>Есть 2 китайских иероглифаб "Ярить" и "Ху". И в правиьлном порядке они имеют огромный смысл.

> Есть 2 китайских иероглифаб "Ярить" и"Ху".
> И в правильном порядке они имеют 

> огромный смысл.


<!--Таблицы(указатель :-- строк нужен только один раз, выравнивать необязательно, маркдаун сам выровняет)-->
| ПН | Вт | Ср | Чт | *Пятница*|
|:---|:---|:---|:---|:---|
|9.00|11.00|15.00|18.00|20.00|
|9.00|11.00|15.00|18.00|20.00|


<!--Вставка кода. код выделяется в обратных кавычках(там где тильда, под ескейпом)-->
Результат выводит команда `console.log`
<!--Если необходимо вставить большой кусок кода, ставим три обратные ковычки до и после кода и можно добавить в строке слово bashб чтобы стал код цветным-->
```bash
def calc(left_operand, right_operand, operation):

    if operation not in ALLOWED_OPERATIONS:
        print("operation is not allowed")
        return None

    try:
        left_operand = int(left_operand)
        right_operand = int(right_operand)
    except ValueError:
        print("Left and right operand must be int")
        return None

    if operation in ["/", "%"] and right_operand == 0:
        print("Division by zero is not allowed")
        return None

    match operation:
        case "+":
            return left_operand + right_operand
        case "-":
            return left_operand - right_operand
        case "*":
            return left_operand * right_operand
        case "/":
            return left_operand / right_operand
        case "%":
            return left_operand % right_operand
        case _:
            print("operation is not supported")
            return None

```

<!--Картинки-->
![Картинка](https://kartynky.com.ua/wp-content/uploads/image_1969.jpg)

<!--кликабельная картинка-->
[![Картинка](https://kartynky.com.ua/wp-content/uploads/image_1969.jpg)](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)
