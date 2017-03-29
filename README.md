# changelog

### 0.1.4 ( 29 Марта 2017 )
   - add: Добавлен путь для установки [slabs-ajaxregistration](https://github.com/Nathan-Stark/slabs-ajaxregistration)

### 0.1.3 ( 23 Марта 2017 )
   - add: Добавлен путь для установки [slabs-ajaxmore](https://github.com/Nathan-Stark/slabs-ajaxmore)

### 0.1.2 ( 20 Марта 2017 )
   - remove: vagrant удален, будет отдельной веткой.
   - add: Добавлен путь для установки [slabs-ajaxform](https://github.com/Nathan-Stark/slabs-ajaxform)
   
### 0.1.1 ( 04 Февраля 2017 )
   - add: Добавлена среда разработки [vagr](https://github.com/Nathan-Stark/vagr)
   - fix: Добавлен в зависемости пакет **composer/installers**

### 0.1.0 ( 22 Января 2017 )   
   - add: Добавлена папка **/web/assets/css/**
   - fix: Исправлено имя папки **assets**
   - fix: Исправлены опечатки в файле **header.php**
   - update: Удалена переменная **BASE_TEMPLATE_PATH** в **define.php**
   - update: Добавлена переменная **BASE_INCLUDE_URL** в **define.php**
   - update: Добавлены расширенные пути composer для компонентов и модулей 1C-bitrix.
   - remove: Удалил **frontend/gulpfile.js** в качестве замены, буду использовать CodeKit
   - remove: Удалил папку **frontend/less/**

## Расширенные пути composer для компонентов и модулей 1C-bitrix
Все сотороние компоненты и модули устанавливаются на прямую в папки local/components/ и local/modules/   
Мои компоненты устаналиваются в local/components/slabs/

## Файловая структура проекта 1C-bitrix
1. **documents** папка, в которой должна содержаться вся документация по проекту.
2. **frontend** папка, в которой будут лежать файлы, необходимые для сборки frontend.
3. **lib** папка, в которой будут лежать файлы классов, которые были написаны специально для проекта.
4. **vendor** папка с библиотеками, загруженными с помощью composer.
5. **web** папка, которая будет доступна из web.
    1. **assets** Папка для стилей, скриптов и картинок
        1. **img** папка с файлами статичных картиновк сайта.
        2. **fonts** папка с подключаемыми шрифтами.
        3. **js** папка с JavaScript скриптами.
    2. **local** папка со всеми компонентами, шаблонами и модулями, которые потребовались для проекта.
        1. **ajax** папска с файлами для ajax запросов.
        2. **include** папка для любых включаемых областей, которые доступны для правки пользователем сайта.
        3. **php_interface** папка с init.php.
            1. **include/agents.php** файл, в котором будут определены все агенты «1С-Битрикс: Управление сайтом».
            1. **include/class.php** файл, в котором будут определены дополнительные классы, нужные проекту.
            2. **include/events.php** файл, в котором будут определены все обраьотчики событий «1С-Битрикс: Управление сайтом».
            3. **include/functions.php** файл, в котором будут определены все дополнительные функции, нужные проекту.
            4. **include/define.php** файл, в котором будут определены все константы, нужные проекту.
            5. **init.php** файл, который подключается при каждом запуске битрикса и подключает файлы из директории "include".
6. **.gitignore** служебный файл git, который исключает некоторый файлы и папки из репозитория.
7. **README.MD** файл в формате [markdown](https://ru.wikipedia.org/wiki/Markdown) с кратким описанием проекта.
8. **composer.json** файл настройки composer.
