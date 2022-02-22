# GitHub_HW_2

1. На локальном репозитории сделать ветки:
+ `git branch Postman`
+ `git branch Jmeter`
+ `git branch CheckLists`
+ `git branch Bag_Reports`
+ `git branch SQL`
+ `git branch Charles`
+ `git branch Mobile_testing`
2. Запушить все ветки на внешний репозиторий
+ `git push -u origin --all`
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
+ `git checkout Bag_Reports` - зайти в ветку Bag_Reports
+ `cat > BagReport_structure.txt`
+ Ввести данные:
```
Summary
Priority
Severity
Status
Environment
Descriprion
  Precondition
   Steps to Reproduce
   Actual Result
   Expected Result
 Attachment
 Assignee
 Reporter
```
+ `ctrl+c` - выход из редактирования
4. Запушить структуру багрепорта на внешний репозиторий
+`git add .; git commit -m "new file"; git push`
5. Вмержить ветку Bag Reports в Main
+ `git checkout main` - перейти в ветку main
+ `git merge Bag_Reports` - вмержить ветку Bag_Reports в main

или одной строкой

+ `git checkout main; git merge Bag_Reports`
6. Запушить main на внешний репозиторий.
+ `git push -u origin main`
7. В ветке CheckLists набросать структуру чек листа.
+ `git checkout CheckLists` - зайти в ветку CheckLists
+ `cat > CheckList_structure.txt`
+ Ввести данные:
```
ID
Title
Precondition
Module
Steps_to_reproduce
Expected_result
Status
```
+ `ctrl+c` - выход из редактирования
8. Запушить структуру на внешний репозиторий
+ `git add .; git commit -m "new file"; git push`
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
+ Перейти на https://github.com/ в репозиторий 
+ Перейти во вкладку Pull Request
+ Нажать кнопку `New pull request`
+ base ветка `main` <-- compare ветка `CheckLists`
+ Нажать `Create pull request`
10. Синхронизировать Внешнюю и Локальную ветки Main
+ `git checkout main; git pull`
