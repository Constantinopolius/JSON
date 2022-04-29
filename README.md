#Homework GitHub_Json
 
4. Создать внешний репозиторий c названием JSON.
Заходим в свой акккунт на GitHub нажимаем кнопку New (зелёная кнопка находиться с лева вверху) )
В поле Repository name вводим имя репозитория JSON скролим до конца страницы и нажимаем кнопку Create repository
Внешний репозитоий создан!

5. Клонировать репозиторий JSON на локальный компьютер.
git clone git@github.com:Constantinopolius/JSON.git (вставляем ссылку скопированую во внешнем репозитории)
 
6. Внутри локального JSON создать файл “new.json”.
cd JSON 
touch new.json
 
7. Добавить файл под гит.
git add new.json
 
8. Закоммитить файл.
git commit -m "add file new.json"
 
9. Отправить файл на внешний GitHub репозиторий.
git push 
 
10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
vim new.json файл откроется в редакторе vim   start new.json в моём случае файл откроется в VisualStudioCode

{
"Full name": "Solovey Konstantsin Sergeevich",
"Age": 32,
"Pet": [{
    "Cat": "pet name buckingham",
    "Breed": "british blue",
    "Age": 8
    }],
"salary 2500"
}

После внесения изменений нажимаем "ESC" для выхода в "командный режим", вводим ":" (двоеточие), вводим "wq" (write-quit) - для сохранения изменений и выхода; "q!" - для выхода без сохранения, и нажимаем "Enter".
Если измения вносились через VSCode сохраняем изменения нажатием клавишь ctrl+s закрываем VScode на кркстик в правом верхнем углу

11. Отправить изменения на внешний репозиторий.
git add new.json
git commit -m "add ifo in file new.json"
git push
 
12. Создать файл preferences.json
touch preferences.json
 
13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
vim new.json файл откроется в редакторе vim   start new.json в моём случае файл откроется в Notepad

{
    "Preferencec": [
      {
        "Movies": [
          "The Wolf of Wall Street",
          "Interstellar",
          "Tenet",
          "Inception"
        ],
        "TV show": [
          "La casa de papel",
          "Mandalorian",
          "Loki"
        
        ],
      "Food":["Fast food"],
      "Seasons":["Summer"],
      "Country":[
        "Barcelona", 
        "Sweeden",
        "United Arab Emirates"
    ]
}
    ]
}

После внесения изменений нажимаем "ESC" для выхода в "командный режим", вводим ":" (двоеточие), вводим "wq" (write-quit) - для сохранения изменений и выхода; "q!" - для выхода без сохранения, и нажимаем "Enter".
Если измения вносились через VSCode сохраняем изменения нажатием клавишь ctrl+s закрываем VScode на кркстик в правом верхнем углу
 
14. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
touch skills.json
vim new.json файл откроется в редакторе vim   start new.json в моём случае файл откроется в Notepad

{
  "Program skills": [
    "SQL",
    "SDLC",
    "STLS",
    "JSON",
    "XML",
    "API",
    "POSTMAN",
    "FIDLER",
    "VPN",
    "DevTools",
    "Android Studio",
    "Charles",
    "Tterminal",
    "Git",
    "Python"
  ],
  "Theoretical knowledge": [
    "Что такое тестирование багрепорты документация виды методы направления тестирования",
    "Что такое клиент серверная архитектура",
    "Методы запросов на сервер",
    "Ответы сервера",
    "Структуры запросов и ответов",
    "Снятие и чтение логов",
    "Мобильное тестирование",
    "Особенность iOS Android гайдлайны",
    "Сборка Android приложений на Android Studio",
    "Сниффинг через Charles",
    "Настройка PROXI на Android and iOS",
    "Доступ к удалённым серверам",
    "Методология разработки Scrum"
  ]
}

После внесения изменений нажимаем "ESC" для выхода в "командный режим", вводим ":" (двоеточие), вводим "wq" (write-quit) - для сохранения изменений и выхода; "q!" - для выхода без сохранения, и нажимаем "Enter".
Если измения вносились через VSCode сохраняем изменения нажатием клавишь ctrl+s закрываем VScode на кркстик в правом верхнем углу

15. Отправить сразу 2 файла на внешний репозиторий.
git add skills.json preferences.json или git add .
git commit -m "add sklls.json preferences.json"
git push 
 
16. На веб интерфейсе создать файл bug_report.json
Заходим в репозиторий JSON на против кнопки с выбором веток main нажимаем на кнопку с 3-мя вертикальными точками 
в выпавшем меню выбираем create new file 
присваеваем имя файлу bag_report 

17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
скролим в низ нажимаем кнопку Commit new file
 
18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
в окно edit new file вносим необходимую нам информацию 
 
{
    "Title": [
        "Summery",
        "Project",
        "Component",
        "Version",
        "Severity",
        "Priority",
        "Status",
        "Author",
        "Assigned To",
        {
            "Environment": [
                "OS",
                "Browser",
                "Browser Version",
                "Service Pack"
            ]
        },
        {
            "Description": [
                "Steps to Reproduce",
                "Expected Results",
                "Actual Results"
            ]
        },
        {
            "Additions": [
                "Attachment"
            ]
        }
    ]
}

19. Сделать (сохранить) изменения на веб интерфейсе.
После добавления информации скролим вниз и нажимаем кнопку Commit changes
 
20. Синхронизировать внешний и локальный репозиторий JSON
git pull 

XML
 
21. Создать внешний репозиторий c названием XML.
 
22. Клонировать репозиторий XML на локальный компьютер.
git clone и вставляем ссылку скопированую во внешнем репозитории
 
23. Внутри локального XML создать файл “new.xml”.
cd .. выходим из репозитория JSON на католог выше 
cd XML 
touch new.xml
 
24. Добавить файл под гит.
git add new.xml 
 
25. Закоммитить файл.
git commit -m "add file.xml"
 
26. Отправить файл на внешний GitHub репозиторий.
git push
