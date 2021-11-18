# LR6
Лабораторная работа №6  
## **Лог команд:**  
cd <*путьдопапки*>  
git config --global user.name "*имяпользователя*"  
git config --global user.email <*email*>  
git clone <*ссылканарепозиторий*>  
git pull  
git checkout <*имяветки*>  
git log 
git merge <*имяветки*>  
git status  
cat <*имяфайла*>  
git add <*имяфайла*>  
git commit -m "*сообщение о коммите*"  
git branch -d <*имяудаляемойветки*>  
git reset --hard <*хэшкоммита*> 
git checkout -b <*имясоздаваемойветки*>  
git push --set-upstream origin <*имяветки*>  
git push  
git push origin -d <*имяветки*>
## **Описание работы:**  
На рабочем столе была создана папка "ЛР6". Необходимо прейти в неё в консоли
![изображение](https://user-images.githubusercontent.com/81923119/142027558-c9b80fa3-88c0-406a-834c-b0a186f110d6.png)  
  
Задаются имя и email пользователя  
![изображение](https://user-images.githubusercontent.com/81923119/142038229-9bf489e0-6c8a-41dd-802b-29ddd12b403f.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142038332-e9a6ed05-aba5-4fa9-ac69-40d8b2c910ac.png)  
  
Удалённый репозиторий клонируется на компьютер  
![изображение](https://user-images.githubusercontent.com/81923119/142040616-f842a7f4-1ca7-4fbe-b498-bb0035446611.png)  
  
Через интерфейс GitHub добавляется файл New File, который заносится в ветку master  
![изображение](https://user-images.githubusercontent.com/81923119/142038599-029ebb40-626b-49ed-bb18-8a4215a57a46.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142038610-f2dad9ce-a853-4f3f-a97f-b204cfccbbc9.png)  
  
Изменения подтягиваются в локальный репозиторий  
![изображение](https://user-images.githubusercontent.com/81923119/142041216-e52501ec-1ecf-4960-9494-70ef32363a66.png)  
  
С помощью команды git log можно получить историю операций для одной из веток, которая является активной. Чтобы переключаться между ветками, используется команда git checkout  
![изображение](https://user-images.githubusercontent.com/81923119/142042061-73b65e6d-f2c4-4fdd-b725-69cfc814cb11.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142042265-0ee12a68-efc9-4853-bb5c-43f8afc92678.png)  
  
Для последующего слияния веток необходимо переключиться на ветку master командой git checkout master. Т.к. есть конфликтующий файл, который можно посмотреть командой git status, то система не даст возможности слияния веток, поэтому необходимо исправить файл и разрешить конфликт командой git add mergefile.txt, а после написать git commit -m "merged and resolved the conflict in mergefile.txt". Так система поймёт, что конфликт урегулирован.  
![изображение](https://user-images.githubusercontent.com/81923119/142046157-f06bb1c5-d4a4-4575-a51e-2f5c49a97978.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142046303-88ff99ab-596d-4133-b3b2-7dfcf6d199fb.png)  
  
После слияния побочная ветка удаляется  
![изображение](https://user-images.githubusercontent.com/81923119/142155168-8950ee79-a184-4b94-b8fa-3d41f73dc837.png)  
  
Добавляются файлы temp.txt и File2.docx и c помощью Блокнота изменяется файл NewFile.txt. После каждого действия производится коммит.  
![изображение](https://user-images.githubusercontent.com/81923119/142155495-ba1f9ed7-b46e-4a02-9fcf-94aade21a90f.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142155855-22638d13-1ccb-4277-9de4-811ee4d9cc03.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142155690-17e896e6-b343-44c4-a077-c46719963626.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142156412-246bf8a1-1fe2-49b4-8cf6-7593c7ddb6d8.png)  

Производится "хард" откат коммита к моменту, когда файл File2.docx не был добавлен, но уже был изменён файл NewFile.txt   
![изображение](https://user-images.githubusercontent.com/81923119/142156771-5c918f12-1798-419b-b064-baa52c9574bf.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142156888-18d37cd1-beb1-45e5-a0b3-b0dced405571.png)  
![изображение](https://user-images.githubusercontent.com/81923119/142158898-5a0d5ad1-514f-4ec8-aac0-5892accaf2d6.png)  

С помощью команды git checkout -b otchet создаётся новая ветка для отчёта.  
![изображение](https://user-images.githubusercontent.com/81923119/142159454-8972a5c3-1602-4018-a0e2-8a8441c8fedc.png)  

Т.к. работа производилась постепенно, то была необходимость в синхронизации локального и удалённого репозитория. Она производилась с помощью различных модификацй команды git push для удаления и добавления веток, а также команды git checkout для переключения между ними  
![изображение](https://user-images.githubusercontent.com/81923119/142159598-5dbe82d9-c9e7-48b8-b31b-e6a98e1c8a20.png)  


