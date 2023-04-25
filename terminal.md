1. Подивитись де я `pdw`
2. Створити папку `mkdir folder1`
3. Зайти в папку`cd folder1`
4. Створити три папки `mkdir folder2 folder3 folder4`
5. Зайти до будь-якої папки `cd folder2`
6. створити 5 файлів(3 txt, 2 json) 
- `touch file1.txt`
- `touch file2.txt`
- `touch file3.txt`
- `touch file1.json`
- `touch file2.json`
7. Створити три папки `mkdir Folder5 Folder6 Folder7`
8. Вивести перелік вмісту папки `ls -la`
9. Відкрити будь-який txt файл 
`nano file1.txt`
10. Написати туди що небудь, будь-який текст
`One of the most critical skills in life, and the value of knowing yourself`
11. Зберегти та вийти
`Ctrl O`
`Enter`
`Ctrl X` 
12. Вийти з папки на рівень вище `cd ..`
13. Перемістити будь які 2 файли, які ви створили, до будь якої іншої папки 
`mv ./folder2/file1.txt ./folder2/Folder6/file11.txt`
`mv ./folder2/Folder6/file11.txt ./file111.txt`
14. скопіювати будь які 2 файли, які ви створили, в іншу якусь папку 
`cp ./folder2/file1.json ./folder2/Folder7/file11.json `
`cp ./folder2/Folder7/file11.json ./file111.json`
15. Знайти файл за допомогою ім'я 
`find -iname "lesson*"`
./folder3/Lesson12Constraint.sql
16. Переглянути вміст у реальному часі (команда grep) вивчіть як вона працює
`tail -f /var/log/syslog | grep -ni --color "gnome"`
17. Вивести кілька перших рядків із текстового файлу
`head -v -n 15 ./folder1/folder3/Lesson12Constraint.sql`
18. Вивести кілька останніх рядків із текстового файлу
`tail -v -n 15 ./folder1/folder3/Lesson12Constraint.sql`
19. Переглянути вміст довгого файлу (команда less) вивчіть, як вона працює.
`less -s /var/log/syslog | grep -i -n "Error"`
20. Вивести дату та час
`date "+%D %T"`
21. Надіслати http запит на сервер http://162.55.220.72:5005/terminal-hw-request
`GET http://162.55.220.72:5005/`

Hello!!!!!!!!!XX.XXX.XX.XXXolv@olv:~$

22. Написати скрипт який виконає автоматично пункти 3, 4, 5, 6, 7, 8, 13
`#!/usr/bin/bash`
`mkdir folder1`
`cd folder1`
`mkdir folder2 folder3 folder4`
`cd folder2`
`touch file1.txt file2.txt file3.txt file1.json file2.json`
`mkdir Folder5 Folder6 Folder7`
`ls -la`
`mv ./file1.txt ./Folder6/file11.txt`
`mv ./Folder6/file11.txt ./file111.txt`

Запустити скрипт 
`sh script.sh`