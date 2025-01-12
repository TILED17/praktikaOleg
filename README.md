# Отчёт по git
Отчет о том как я использовал программу git для выгрузки и загрузки файлов с сервера GitHub
<p align="center">
  <img style="background-color: white;" width="400" height="400" src="https://gitlab.com/e.s.s.e.e.system/test_project_2/-/raw/master/logo.png?ref_type=heads">
</p>

----

## Шаг 1
Сперва нужно скачать саму программу.

Вот ссылка на скачивание: [https://git-scm.com/downloads/win](https://git-scm.com/downloads/win)

После того как скачали, устанавливаем ничего не меняя в параметрах установки.

## Шаг 2
Если нажать по ПКМ (Правой кнопкой мыши), то можно увидеть что у нас появился дополнительно два пункта в меню:
1. Open Git Gui here
2. Open Git Bash here

В данном отчете мы не будем рассматривать эти пункты, моя задача обьяснить как выгрузить и загрузить свои проекты

Создайте новый репозиторий в GitHub и скопируйте ссылку на него.

## Шаг 3 
Для ознакомления с данной программой советуется попрактикоаться с пустым проектом.

Создайте новую папку и в нем же создайте текстовый документ, чтобы папка не казалось пустым.

## Шаг 4
В этой же папке, ПКМ-ом открываем терминал и пишем следующую команду:

      git clone [Ссылка на ваш репозиторий]

В квадратных скобках вставляем ссылку без этих скобок

Данная команда копирует все файлы с сервера, точнее с вашего репозитория на папку, которого вы недавно создали. Можно считать это как загрузкой, причем загрузить можно любые репозитории на сайте GitHub которые есть, но при условии, если автор не сделал его публичным.

## Шаг 5
Чтобы выгрузить файлы с нашей папки нужно соединиться со сервером.

На том же терминале пишем следующую команду: 

    git remote add origin [Ссылка на ваш репозиторий]

Данная команда позволяет соединиться с вашим репозитроием на GitHub.

#### Внимание!
У вас должно появиться окно где нужно войти в свой аккаунт GitHub. Заполняем логин, пароль и заходим.

## Шаг 6
После того как зашли, то можно уже выгружать свой проект в сервер GitHub.

Пишем следующую команду на том же терминале:

    git push origin master

master - это главная ветка по умолчанию

### Поздравляю!
Вы успешно выгрузили текстовый документ с папки на ваш проект в сервере.

## Дополнительно
Так как я упомянул про ветки, чтобы их создать прописываем следующую команду в терминале:

    git branch [Имя новой ветки]

На квадратных скобках пишем имя новой ветки (Сами квадратные скобки мы убираем)

По умолчанию, когда загружаете файлы в сервер, вы находитесь на ветке *master*, чтобы переключится на другую ветку пишем следующую команду:

    git checkout [Имя ветки]

Вот и все, вы успешно перешли на другую ветку можете дальше выгружать в этой ветке с соответствующей командой:

    git push origin [Имя ветки]
