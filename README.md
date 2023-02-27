# Превое домашнее задание - знакомство с командами git.
1) Посмотреть где я - pwd

2) Создать папку - mkdir folder_1

3) Зайти в папку - cd folder_1

4) Создать 3 папки - mkdir f1 f2 f3

5) Зайти в любоую папку - cd f1

6) Создать 5 файлов - (3 txt, 2 json) - touch first.txt second.txt third.txt fourth.json fifth.json

7) Создать 3 папки - mkdir fold_1 fold_2 fold_3

8) Вывести список содержимого папки - ls -la

9) Открыть любой txt файл - cat >> first.txt

10) написать туда что-нибудь, любой текст. - 
row1
row2
row3

11) сохранить и выйти. - CTRL + C

12) Выйти из папки на уровень выше - cd ..

13) переместить любые 2 файла, которые вы создали, в любую другую папку. - mv f1/first.txt f1/fourth.json f2

14) скопировать любые 2 файла, которые вы создали, в любую другую папку. - cp f1/second.txt f1/fifth.json f1/fold_2

15) Найти файл по имени -  find . -name second.txt

16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. - tail -f f2/first.txt
- Зайти в файл first.txt в Windows
- Внести в него изменения в Windows
- Нажить CTRL + S в Windows
- В консоле увидеть изменения в файле в реальном времени
-Выйти из файла нажатием CTRL + C в консоли

17) вывести несколько первых строк из текстового файла - head -2 f2/first.txt

18) вывести несколько последних строк из текстового файла - tail -2 f2/first.txt

19) просмотреть содержимое длинного файла (команда less) изучите как она работает. - less f1/second.txt

20) вывести дату и время - date

1*) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request - curl "http://162.55.220.72:5005/terminal-hw-request"

2*) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 --- 
-создаем заранее папку for_script где будут выполняться команды и созданные файлы скрипта
-vim myscript.sh
-вписываем в него скрипт:
#!/bin/bash
cd for_script
mkdir folder_2 folder_3 folder_4
cd folder_2
touch file_1.txt file_2.txt file_3.txt file_4.json file_5.json
mkdir folder_5 folder_6 folder_7
ls -la
cd ..
mv folder_2/file_1.txt folder_2/file_4.json folder_3
-сохраняем и запускаем скрипт командой:
bash myscript.sh
