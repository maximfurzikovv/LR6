# LR6
## Лабораторная работа №6
### Цель лабораторной работы: изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.  

### 1. Создание аккаунта на сайте GitHub
В работе использовался уже имеющийся аккаунт на сайте GitHub. На сайте была сделана копия из https://github.com/Kurtyanik/LR6/ (Fork). С помощью GitBash были изменены имя и почта. (см. рис. 1)  
![image](Git/1.png)  
Рисунок 1 - Изменение имени пользователя и почты
### 2. Клонирование удаленного репозитория на комьютер
Клонирование репозитория было выполнены с помощью команды git clone (см. рис. 2).  
![image](Git/2.png)  
Рисунок 2 - Клонирование репозитория  
### 3. Добавление файла через интерфейс GitHub
В ветке master с помощью интерфейса GitHub был создан файл "NewFile.txt". С помощью команды git pull origin master изменения были подтянуты в локальный репозиторий (см. рис. 3).  
![image](Git/3.png)  
Рисунок 3 - Добавление файла и подтягивание изменений  
### 4. Получение истории операций для каждой из веток
С помощью git log --all были получены истории операций для каждой из веток (см. рис. 4).  
![image](Git/4.png)  
Рисунок 4 - История операций  
### 5. Просмотр последних изменений.
Для просмотра последних изменений была использована команда git show (см. рис. 5).  
![image](Git/5.png)  
Рисунок 5 - Просмотр последних изменений.  
### 6. Слияение в ветку master с разрешением конфликта
Затем было выполнено слияние в ветку master с помощью команды git merge origin/branch1 origin/master (см. рис. 6). Возник конфликт, для разрешения которого были удалены некоторые данные из файла mergefile.txt.  
![image](Git/6.png)  
Рисунок 6 - Слияние веток  
Данные изменения были сохранены (см. рис. 7).  
![image](Git/7.png)  
Рисунок 7 - Сохранение изменений  
### 7. Удаление побочной ветки после успешного слияния
С помощью git push origin --delete branch1 была удалена побочная ветка (см. рис. 8).  
![image](Git/8.png)  
Рисунок 8 - Удаление побочной ветки  
### 8. Выполнение изменений и их фиксирование
Затем, в файл mergefile.txt были внесены изменения, которые позже были зафиксированы (см. рис. 9).  
![image](Git/9.png)  
Рисунок 9 - Внесение изменений и их фиксирование.  
### 9. Откат коммита
Затем был осуществлен откат коммита - git revert c06f031 (см. рис. 10).  
![image](Git/10.png)  
Рисунок 10 - Откат коммита  
### 10. Создание ветки для отчета
![image](Git/11.png)  
Рисунок 11 - Создание ветки report для оформления отчета  
### 11. История операций в форматированном виде
![image](Git/12.png)  
Рисунок 12 - История операций для ветки master  
![image](Git/12.1.png)  
Рисунок 13 - История операций для ветки report  
### 12. Лог команд
git config - функция используется для настройки значений конфигурации Git на глобальном и локальном уровнях проекта.  
git clone - команда клонирует репозиторий в новую локальную директорию.  
git pull - функция используется для извлечения только что полученной информации и ее загрузки в локальной репозиторий.  
git log - команда выводит список коммитов в репозитории.  
git show - команда показывает информацию о конкретном коммите.  
git merge - команда используется для объединения двух веток.  
git commit -m - команда совершает коммит (закрепляет промежуточные результаты).  
git push - команда передаёт в удалённый репозиторий изменения, сделанные в локальном репозитории.  
git add . - команда переносит все новые и измененные файлы в раздел проиндексированных файлов.  
git revert - команда создает новый коммит, который отменяет изменения указанного коммита.  
git branch - команда выводит список веток в репозитории.  
git checkout - команда используется для переключения ветки.  
git log --pretty=format:"%h + %cd +%an + %s" - команда устанавливает пользовательский формат вывода лога.  
### Вывод: были изучены базовые возможности системы управления версиями, получен опыт работы с Git Api, с локальным и удаленным репозиторием.
