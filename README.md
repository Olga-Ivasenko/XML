## **Repository 2 XML**
**21. Создать внешний репозиторий c названием XML**
- **version via GitHub**:
	- push `NEW` button
	- enter repository name "XML"
	- choose a `README file` option
	- push `Create repository` button
	-
- **version via Terminal for authenticated users only**:
	- use API link to send POST request:
[API link](https://api.github.com/)
	- enter the command:
```bash
curl -u "YourGitHubName" https://api.github.com/user/repos -d "{"name":"XML","public": true}"
```
	- enter your password
	- under response find URL named "clone_url": and copy it
	- go to GitHub by copied link and find your new repository

- **version via Terminal for any user**:
```bash
mkdir XML
cd JXML
git init
touch README.md
git commit -m "commit of xml"
```
```bash
git remote add origin 
git@github.com:YourGitHubName/<XML>.git
```
```bash
curl -u YourGitHubName:YourTokinORYourPassword https://api.github.com/user/repos -d '{"name":"XML"}'
```

**22. Клонировать репозиторий XML на локальный компьютер**
- copy link of repository under `Code` button
![Commit button](https://github.com/Olga-Ivasenko/XML/blob/24c6abef4919c79e192818fb66cba27828fc506a/edit_picture5.jpg)
- commands:
```bash
cd MyDirectory	//where new project to be placed locally
git clone + <copied link>
```

**23. Внутри локального XML создать файл “new.xml”**
```bash
cd XML
touch new.xml
```
**24. Добавить файл под гит**
```bash
git add new.xml // to add exact file
git add . // to add all files
```
**25. Закоммитить файл**
```bash
git commit -m "xml commit"
```
**26. Отправить файл на внешний GitHub репозиторий**
```bash
git status
git push
```
**27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML**

```bash
cd XML
vim new.xml
```
- enter xml data:
[XML data](https://github.com/Olga-Ivasenko/XML/blob/d615646cd198ea77897f01d732ebde7e5a90762b/new.xml)

**28. Отправить изменения на внешний репозиторий**
```bash
git status
git commit -m "new xml changes" // if all added files
git commit -m "new xml changes" new.xml // if selected file
git push
```

**29. Создать файл preferences.xml**
```bash
cd XML
touch preferences.xml
```

**30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML**
```bash
cd XML
vim preferences.xml
```
- enter xml data:
[XML data](https://github.com/Olga-Ivasenko/XML/blob/0eff3fc73c1f8bc478b039584fd544ea9c329e3f/preferences.xml)


**31. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML**
```bash
cd XML
touch sklls.xml
vim sklls.xml // or without touch but save before closing
```
- enter xml data
[XML data](https://github.com/Olga-Ivasenko/XML/blob/0eff3fc73c1f8bc478b039584fd544ea9c329e3f/skills.xml)

**32. Сделать коммит в одну строку**
```bash
cd XML
git status
git add skills.xml
git add preferences.xml
git status
git commit -m "add two files" skills.xml preferences.xml
```

**33. Отправить сразу 2 файла на внешний репозиторий**
```bash
git push
```
**34. На веб интерфейсе создать файл bug_report.xml**
- go to GitHub, repository you`ve created
- push `Add File` dropdown button
- choose `Create new file`
![Commit button](https://github.com/Olga-Ivasenko/XML/blob/24c6abef4919c79e192818fb66cba27828fc506a/edit_picture4.jpg)
- name your file "bug-report.xml"

**35. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- choose `Edit new file` tab
- enter \{} to the edit field of the file
- choose `Preview` tab
- push `Commit your file` button
![Commit button](https://github.com/Olga-Ivasenko/XML/blob/24c6abef4919c79e192818fb66cba27828fc506a/edit_picture3.jpg)

**36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML**
- go to main branch of repository
- step on your file "bug-report.xml"
- choose `edit` pictogram
![how to find Edit](https://github.com/Olga-Ivasenko/XML/blob/24c6abef4919c79e192818fb66cba27828fc506a/edit_picture1.jpg)
- enter xml data:
[XML data](https://github.com/Olga-Ivasenko/XML/blob/0eff3fc73c1f8bc478b039584fd544ea9c329e3f/bug_report.xml)

**37. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- go down of edit file page
- *optional*: add description
- click `Commit changes` button
![Commit button](https://github.com/Olga-Ivasenko/XML/blob/24c6abef4919c79e192818fb66cba27828fc506a/edit_picture2.jpg)

**38. Синхронизировать внешний и локальный репозиторий XML**
```bash
cd XML
git pull
git add .
git status
git commite -m
git push
```
