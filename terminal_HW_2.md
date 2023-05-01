1. Сделать папку dir_1
`mkdir dir1`

2. Зайти в папку dir_1
`cd ./dir_1`

3. Создать папку inner_dir_1
`mkdir inner_dir_1`

4. Посмотреть где ты находишься
`pwd`

5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt
`touch tf_1.txt`

6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:
`- the first 1`
`- the second 2`
`- the third 3`

`cat > tf_2.txt`
> -the first 1
-the second 2     
-the third 3

`Ctrl d`

7. Зайти в папку inner_dir_1
`cd ./inner_dir_1`

8. Через cat сделать текстовый файл tf_3.txt  c любыми строками
`cat > tf_3.txt`
> Cat
Dog
Rat

9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2”
`cat >> tf_3.txt`
> "the second 2"

10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”
`cat >> tf_3.txt`
> "the sec 2"

11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”
`cat >> ~/dir_1/tf_2.txt`
> "the sec 3"

12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”
`cat >> tf_3.txt`
> "the SeCoNd 2"

13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”
`cat >> ~/dir_1/tf_2.txt`
> "the seConD 2"

14. Сделать текстовый файл tf_4.txt в котором будет 15 строк.
`nano tf_4.txt`
`Enter` 15 раз
`Ctrl o`
`Enter`
Wrote 15 lines
`Ctrl x`

15. Сделать текстовый файл tF_5.txt в котором будет 13 строк.
`tail -n 13 tf_4.txt > tF_5.txt`

16. Вывести список всех файлов в папке.
`ls -la`

17. Выйти из папки inner_dir_1
`cd ..`

18. Вывести содержимое файла tf_3.txt в терминал.
`cat ./inner_dir_1/tf_3.txt`
> Cat
Dog
Rat
"the second 2"
"the sec 2"
"the SeCoNd 2"

19. Найти путь к файлу tf_4.txt
`find -name tf_4.txt`
> ./inner_dir_1/tf_4.txt

20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.
`truncate -s 0 tf_4.txt`

21. Найти путь к файлам у которых есть  “tf” в названии.
`find -name "*tf*"`
> ./tf_4.txt
./tf_2.txt
./tf_1.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tf_3.txt

22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре.
`find -iname "*tf*"`
> ./tf_4.txt
./tf_2.txt
./tf_1.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tF_5.txt
./inner_dir_1/tf_3.txt

23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке
`grep "sec" ./*.*`
> ./tf_2.txt:-the second 2
./tf_2.txt:"the sec 3"

24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке
`grep -i "sec" ./*.*`
> ./tf_2.txt:-the second 2
./tf_2.txt:"the sec 3"
./tf_2.txt:"the seConD 2"

25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке
`grep -w "sec" ./*.*`
> ./tf_2.txt:"the sec 3"

26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке
`grep -wi "sec" ./*.*`
> ./tf_2.txt:"the sec 3"

27. Найти строки в файлах где есть комбинация букв “second” в текущей папке
`grep "second" ./*.*`
> ./tf_2.txt:-the second 2

28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке
`grep -i "second" ./*.*`
> ./tf_2.txt:-the second 2
./tf_2.txt:"the seConD 2"

29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем
`grep -r "second"`
> tf_2.txt:-the second 2
inner_dir_1/tf_3.txt:"the second 2"

30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке
`grep -l "second" ./*.*`
> ./tf_2.txt

31. Найти все строки во всех файлах где нет комбинации “second”
`grep -vri "second"`

> tf_2.txt:-the first 1
tf_2.txt:-the third 3
tf_2.txt:"the sec 3"
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tf_3.txt:Cat
inner_dir_1/tf_3.txt:Dog
inner_dir_1/tf_3.txt:Rat
inner_dir_1/tf_3.txt:"the sec 2"

32. Найти только название и путь к файлам где нет комбинации “second”
`grep -vril "second"`
> tf_2.txt
inner_dir_1/tf_4.txt
inner_dir_1/tF_5.txt
inner_dir_1/tf_3.txt

33. Вывести в терминал 4 последних строк любого текстового файла
`tail -n 4 ./inner_dir_1/tf_3.txt`
>Rat
"the second 2"
"the sec 2"
"the SeCoNd 2"

34. Вывести в терминал 4 первые строки любого текстового файла.
`head -n 4 ./inner_dir_1/tf_3.txt`
Cat
Dog
Rat
"the second 2"

35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.
`mkdir Privet | echo Hello > privet.txt`
`ls -t` 
> Privet  privet.txt inner_dir_1  tf_4.txt  tf_2.txt  tf_1.txt

36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
`find . -type f -name "*.txt" -print0 | xargs -0 grep -lZ "sec" | xargs -0 -I {} mv {} ~/dir_1/`
>ls -t
inner_dir_1  Privet  privet.txt  tf_4.txt  tf_3.txt  tf_2.txt  tf_1.txt

37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
`find . -type f -name "*.txt" -print0 | xargs -0 grep -lZ "sec" | xargs -0 -I {} cp {} ~/dir_1/Privet/`
> cd ./Privet/
ls -t
tf_2.txt  tf_3.txt

38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.
`find . -type f -name "*.txt" -print0 | xargs -0 grep -hFZ "sec" | xargs -0 > new1.txt`
> cat new1.txt
"the second 2"
"the sec 2"
- the second 2
'the sec 3"
"the second 2"
"the sec 2"
"the second 2"
"the sec 2"
- the second 2
'the sec 3"

39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”
`find . -type f -name "*.txt" -print0 | xargs -0 grep -l "sec" | xargs rm`

40. Просто вывести в терминал строку “Good job!!”
`echo '"Good job!!"'`
>"Good job!!"
