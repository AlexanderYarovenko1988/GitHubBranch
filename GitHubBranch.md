1. На локальном репозитории сделать ветки для:
- Postman
>git branch Postman
- Jmeter
>git branch Jmeter
- CheckLists
>git branch CheckList
- Bag Reports
>git branch BagReports
- SQL
>git branch SQL
- Charles
>git branch Charles
- Mobile testing
>git branch MobileTesting

2. Запушить все ветки на внешний репозиторий
>git push -u --all
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
>git checkout BugReports && vim bag.txt
4. Запушить структуру багрепорта на внешний репозиторий
>git add . && git commit -m "bag" && git push
5. Вмержить ветку Bag Reports в Main
>git checkout main && git merge BagReports
6. Запушить main на внешний репозиторий.
>git push
7. В ветке CheckLists набросать структуру чек листа.
>git checkout CheckLists && vim checklist.txt
8. Запушить структуру на внешний репозиторий
>git add . && git commit -m "checklist" && git push
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
>GitHub -> CheckLists had recent pushes less than a minute ago -> Compare && Pull requests -> Pull request successfully merged and closed
10. Синхронизировать Внешнюю и Локальную ветки Main
>git checkout main && git pull
