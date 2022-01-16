# JSON
First HW GitHub
 4. Создать внешний репозиторий c названием JSON.
 GitHub > Repositories > New > JSON
 5. Клонировать репозиторий JSON на локальный компьютер.
 git clone https://github.com/Ollika-Polika/JSON.git
 6. Внутри локального JSON создать файл “new.json”.
 cat > new.json
 "employee": {
        "name":       "Bill",
        "salary":      56000,
        "married":     true
 }
 7. Добавить файл под гит.
 git add new.json
 8. Закоммитить файл.
 git commit -m "new.json adding for the first time"
 9. Отправить файл на внешний GitHub репозиторий.
 git push
 10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
 vim new.json
 {
		"employeeID": 1,
        "name":       "Bill",
        "salary":     56000,
        "married":    true
 }

 {
		"employeeID": 2,
        "name":       "Olli",
        "age":        27,
        "animals":    1,
        "salary":     1000000
 }
 /save and exit - :wq
 11. Отправить изменения на внешний репозиторий.
 git commit -am "add my employee2 information"
 git push
 12. Создать файл preferences.json
 touch preferences.json
 13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
 vim preferences.json
 "preferences": [
        "fav_movie":     "The_Irony_of_Fate",
        "fav_serial":    "Friends_EN",
        "fav_food":      "vegetarian_dishes",
        "fav_season":    "summer",
        "fav_country":   "Iceland"
 ]
 14. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
 touch sklls.json
 vim sklls.json
 "skills": [ "GitBash_Terminal", "GitHub", "API", "SQL", "Jmeter", "HTTPmethods", "JSON", "XML", "Charles", "Fidler", "VPN", "iOS_with_X-code", "Android_Studio", "PostgresDB", "Redis", "Python" ]
 15. Отправить сразу 2 файла на внешний репозиторий.
 git add .
 git commit -m "add both json files with preferences and skills"
 git push
 16. На веб интерфейсе создать файл bug_report.json.
 JSON > Add file > Create new file > JSON/bug_report.json
 "Bug report id": {
         "id": 1,
         "title": "Chat - User cannot rename group conversation"
 }
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Comment for commit: add bug_report with bug report id information
 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
 Click bug_report.json > edit 
 "Bug report id": {
         "ID":    1,
         "Title": "Chat - User cannot rename group conversation"
 }
 "Details": {
         "Type":  "Bug",
         "Priority": "Medium",
         "Affects_Version": "None",
         "Component": "None",
         "Labels": "None",
         "Sprint": "S22"
 }
 "Description": {
         "Steps_to_reproduce": {
                  1: "Log in",
                  2: "Open chat dialog",
                  3: "Click on the Setting button",
                  4: "Add user",
                  5: "Add user to a group conversation",
                  6: "Try to rename this group conversation"
         }
         "Expected_result": "User can rename group conversation",
         "Actual_result": "Rename conversation button is disabled"
 }
 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Comment for commit: Update bug_report.json
 20. Синхронизировать внешний и локальный репозиторий JSON
 git fetch - проверка обновлений на внешнем репозитории
 git pull - синхронизация
