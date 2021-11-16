# LR6
Лабораторная работа №6  
## **Лог команд:**  
cd -  
git config --global user.name ""  
git config --global user.email <>  
git clone  
git pull  
git checkout
git log 
git merge  
git status  
cat  
git add  
git commit -m "information about commit"  
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


Добавляются файлы  и изменяется файл . После каждого действия производится коммит.  


Производится "хард" откат коммита к моменту, когда файл не был добавлен, но уже был изменён файл  

