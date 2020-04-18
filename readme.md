# NeuroStartUp теперь в GitHub
![Neuro Logo](https://camo.githubusercontent.com/c6727c717cad1e4820481abb87524f90782445c5/68747470733a2f2f692e696d6775722e636f6d2f495a4f525769492e706e67)

NeuroStartUp — динамически развивающийся стартап, специализирующийся на поиске с использованием новейших технологий искусственного интеллекта.

## Наши преимущества:
1. Высокая точность поиска
1. Высокая скорость поиска
1. Низкая цена


### Для работы потребуется:
1. Скачать и установить на локальной машине программу Git(Ссылки в описании ниже )
1. Настроить программу Git для работы (смотри описание ниже)
1.  Зарегистрироваться на сайте - [GitHub](https://github.com)

 *Для удобства работы с файлами можно так же скачать специальную программу. Например: Visual Studio Code*
### Установка и запуск
#### Для скачивания программы Git:

* Windows-[Перейти по ссылке](https://git-scm.com/download/win)
* Mac-[Перейти по ссылке](https://git-scm.com/download/mac)
* Ubuntu-Запустить в коммандной строке - apt-get install git
* Fedora-Запустить в коммандной строке- dnf install git 
* Другие версии Linux-[Перейти по ссылке](https://git-scm.com/download/linux)

#### Первые настройки в программе Git:
* Для этого, после установки Git, в проводнике выбираете нужную папку-Нажимаете правой кнопкой мышки-Выбираете "Git Bash Here"
* Запустить в открывшемся окне:
    1. git config --global user.name "Указать свое имя"
    1. git config --global user.email Прописатьпочту
    * Рекомендация: запустить строчку git config --global core.editor nano
 

### Начало работы:

* Действующий проект - [NeuroStartUP](https://github.com/YuryFedoseev/NeuroStartUp.git). На данной странице будут отображаться все отправленные изменения по проекту
* Далее всем желающим работать с проектом потребуется скопировать проект себе на лкальную машину.Для этого потребуется:
    1. скопировать ссылку на проект.
         * Либо взять ссылку из прошлого пункта;
         * Либо  Найти кнопку "Clone or download" (Обычно зеленого цвета, Находится с правой стороны под панелью работы с данным проектом) и скопировать ссылку от туда.
    1. запустить на своей локальной машине программу Git в той папке, куда хотите загрузить проект(Для этого, после установки Git, в проводнике выбираете нужную папку-Нажимаете правой кнопкой мышки-Выбираете "Git Bash Here")
    1. В открывшемся окне запустить команду- git clone --вставить ссылку, скопированную ранее-- 

## Результат:
На вашей локальной машине, в нужной вам папке появился проект, с которым вы теперь можете работать.




### После выполнения всех, указанных выше, действий у вас на локальной машине будет копия проекта. Все участники проекта смогут работать с общими файлами, вводя необходимые изменения и комментарии.

Для примера:
* созданы файлы Oplata.txt, bisnesplan.txt и kontakt.xlsx
* в данных файлах заполнили некоторые данные
* мы добавили эти файлы в Git командой git add * (т.к. нам нужны все эти файлы. Можно было поочередно перечислить все указанные файлы)
* добавили коментарий командой git commit -a -m "Новые файлы Оплаты, бизнес плана, контактов"
* выполнили команду git push
#### Результат:
Все файлы, которые мы добавили и все, что мы прописали теперь доступно к загрузке с любого другого компьютера нужного вам сотрудника.На сайте в действующем проекте теперь можно увидеть кто, когда и что именно добавил.
Другие участники проекта могут изменить существующие файлы, добавить новые и т.д. Так командная работа будет проще, безопаснее и зеркальнее. Каждый участник в любое время может посмотреть, на каком этапе находится проект. В случае необходимости у вас будет возможность вернуть проект к моменту до возникновения какой-либо ошибки, изменения и т.д.



### Краткий сбор команд для Git
1. git init
    * требуется для создания нового локального репозитория. В данном случае не требуется т.к. репозиторий скопирован с GitHub)
1. git add index.html
    * где index.html- это имя добавляемого в работу   файла
    * можно использовать расширенное добавление: git add * (добавит в отслеживание все файлы из используемой папки) или git add *.js (добавит в отслеживание все файлы с нужным расширением из используемой папки)
1. git status
    * позволяет отследить текущий статус вашего
репозитория
1. git commit
    * команда для фиксации изменений. После запуска данной команды откроетя редактор для указания комментария
    * для того, чтобы сразу сохранять комментарий можно запустить команду git commit -a -m "Прописать сюда комментарий"
        * Флаг -a ( --all ) говорит о том, что мы добавляем в stage все
удалённые/изменённые файлы (но не новые, новые нужно добавлять
отдельно).
Флаг -m "Сообщение коммита" ( --message="Сообщение
коммита" ) позволяет не открывать редактор, а указывать сообщение
прямо в командной строке.

1. git log
    * команда для просмотра истории комитов
1. git rm --cached stuff.txt
    * команда для удаления файла из stage area.
    * stuff.txt – имя нужного файла.
1. git commit --amend -m "Roboto Font"
    *Программа для исправления последнего комментария коммита. 
    * "Roboto Font" – новое сообщение коммита   
1. git
    * краткая справка по git
1. git help <command>
    * справка по конкретной команде git
1. git push
    * команда для отправки данных на GitHub
    * Первый раз нужно запускать:
        * git push –u origin master
    * Далее всегда просто git push


Подробнее по работе с программой Git, расширенные настройки и другие команды вы можете узнать на онлайн курсах [Университета Нетология](https://netology.ru/) 