# Git

## HomeWork 2


**1. На локальном репозитории сделать ветки для:**
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing
```bash
git branch Postman
git branch Jmeter
git branch CheckLists
git branch Bug-reports
git branch SQL
git branch Charles
git branch Mobile_testing
```
**2. Запушить все ветки на внешний репозиторий:**
```bash
git push -u origin --all
```
**3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта:**
```bash
git checkout Bug_reports
cat > br.txt
[Enter]
№: DL_01
Title: White screen is displayed after tapping 'Free chest' icon in the store
Environment: Huawei P30 Pro, Android 10
Precondition: The app is lounched
Inputs: Login 1 Pass 123
Steps to reproduce:
    1) Tap 'Store' icon.
    2) Tap 'Free chest' icon.
Expected result: The screen with the number of diamonds received is opened
Actual result: White screen is displayed
Severity: Major
Priority: Medium
Attachments: None
[Enter]
[Ctrl + C]
```
**4. Запушить структуру багрепорта на внешний репозиторий:**
```bash
git add .
git commit -m "br.txt"
git push
```
**5. Вмержить ветку Bag Reports в Main:**
```bash
git checkout main
git merge Bug-reports
```
**6. Запушить main на внешний репозиторий:**
```bash
git push
```
**7. В ветке CheckLists набросать структуру чек листа:**
```bash
git checkout CheckLists
cat > checklist_01.txt
[Enter]
Check List
№ DL_01

1. Установить приложение
2. Открыть приложение
3. Зарегистрироваться
4. Залогиниться
5. Выполнить упражнение
6. Открыть бесплатный сундук
7. Купить алмазы
8. Купить усиление
9. Купить платную версию
[Enter]
[Ctrl + C]
```
**8. Запушить структуру на внешний репозиторий**
```bash
git add .
git commit -m "checklist_01.txt"
git push
```
**9. На внешнем репозитории сделать Pull Request ветки CheckLists в main**
```bash
[Pull requests] > [Compare & pull request] > [Create pull request] > [Merge pull request]
```
**10. Синхронизировать Внешнюю и Локальную ветки Main**
```bash
git checkout main
git pull
```
---