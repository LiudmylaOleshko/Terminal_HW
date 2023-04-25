1.. Заголовки

`#` 
# text
`##` 
## text
`###` 
### text
`####`
#### text
`#####`
##### text
`######` 
###### text
2.. Разделение 

`=========`

3.. Выделение текста
`*курсив*`
*курсив*
`**жирный**`
**жирный**
`***жирный курсив***`
***жирный курсив***
3.. Выделение блоков
`______________`
_______________
`--------------`
---------------

4.. Зачеркнутый текст
`~~**text**~~`
~~**text**~~

5.. Не нумерованнные списки любым из 3 способов
`+ Англия`
`+ Италия`
`+ Германия`
+ Англия
+ Италия
+ Германия

`* США`
`* Мексика`
`* Бразилия`
* США
* Мексика
* Бразилия

`- Греция`
`- Италия`
`- Испания`
- Греция
- Италия
- Испания

6.. Нумерованные списки, если начинаем с 1 то все последующая нумерация по-порядку, чтобы мы не писали

`1. Англия`
`2. Италия`
`3. Испания`
`10. Франция`
`1. Греция`
`18. Германия`
1. Англия
2. Италия
3. Испания
10. Франция
1. Греция
18. Германия

7.. Если на чинаем с другой цифрыб например 50, то и номерация будет продолжаться с 50 и далее попорядку-->
`50. США`
`12. Мексика`
`25. Бразилия`

50. США
12. Мексика
25. Бразилия

8.. Вложенные списки
`1. Англия`
`    * Бигбег`
`   * Мини купер`
`    * Автобус`
`2. Италия`
`3. Франция`

1. Англия
    * Бигбег
    * Мини купер
    * Автобус
2. Италия
3. Франция

9.. Ссылки
`[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)`
[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)
9.1 Если хотим подсказку при подсвечивании ссылки
`[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/`
[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/ "Мой линкедин")

`Здравствуйтеб это мой линкедин: <[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)>`
Здравствуйтеб это мой линкедин: <[Linkedin](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)>

10.. Цитаты
`>Есть 2 китайских иероглифа, "Ярить" и "Ху". И в правильном порядке они имеют огромный смысл.`
>Есть 2 китайских иероглифа, "Ярить" и "Ху". И в правильном порядке они имеют огромный смысл.

`> Есть 2 китайских иероглифа, "Ярить" и"Ху".`
`> И в правильном порядке они имеют` 
`> огромный смысл.`
> Есть 2 китайских иероглифа, "Ярить" и"Ху".
> И в правильном порядке они имеют 
> огромный смысл.

11.. Таблицы(указатель :-- строк нужен только один раз, выравнивать необязательно, маркдаун сам выровняет)
`| ПН | Вт | Ср | Чт | *Пятница*|`
`|:---|:---|:---|:---|:---|`
`|9.00|11.00|15.00|18.00|20.00|`
`|9.00|11.00|15.00|18.00|20.00|`
| ПН | Вт | Ср | Чт | *Пятница*|
|:---|:---|:---|:---|:---|
|9.00|11.00|15.00|18.00|20.00|
|9.00|11.00|15.00|18.00|20.00|

12.. Вставка кода. код выделяется в обратных кавычках(там где тильда, под ескейпом)
Результат выводит команда 
`console.log`

13.. Если необходимо вставить большой кусок кода, ставим три обратные ковычки до и после кода и можно добавить в строке слово bash, чтобы стал код цветным 
>  '''  big code ''' (только ковычки используем такие: `````````)

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

14.. Картинки
`![Картинка](https://kartynky.com.ua/wp-content/uploads/image_1969.jpg)`
![Картинка](https://kartynky.com.ua/wp-content/uploads/image_1969.jpg)

15.. Kликабельная картинка
`[![Картинка](https://kartynky.com.ua/wp-content/uploads/image_1969.jpg)](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)`
[![Картинка](https://kartynky.com.ua/wp-content/uploads/image_1969.jpg)](https://www.linkedin.com/in/liudmyla-oleshko-a4a560222/)
