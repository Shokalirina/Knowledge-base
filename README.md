# РУКОВОДСТВО ПО УСТАНОВКЕ БЗ ИСС по Истории г.Минска

###	1. КЛОНИРОВАНИЕ ПРОЕКТОВ
Для клонирования установочных скриптов необходимо создать каталог для нашего проекта и перейти в него. В руководстве будем клонировать проекты в корневую папку (Home). 

Для загрузки установочных скриптов выполняем команду:
* git clone https://github.com/ShunkevichDV/ostis.git

Данная команда создаст в корневой дериктории папку «ostis/scripts». Перейдем в нее, выполнив в терминале команду:
* cd ostis/scripts

Далее запустим скрипт «prepare.sh», который склонирует необходимые проекты (sc-machine, sc_web и др.) в папку «ostis», а также создаст скрипты для запуска. Выполним команду:
* ./prepare.sh

Возвращаемся на одну директорию назад и переходим в папку kb:
* cd ..
* cd kb
 
Удаляем папку menu:
* rmdir -rf menu

Клонируем Базу знаний проекта по Истории
* git clone https://github.com/Historicteam/Knowledge-base.git
		
### 2. СБОРКА И ЗАПУСК ПРОЕКТА
Переходим в папку scripts:
* cd ..
* cd scripts

Для сборки базы выполняем скрипт:
* ./build_kb.sh

Запускаем sctp сервер, выполнив команду в терминале:
* ./run_sctp.sh
 
В новом окне терминала (CTRL + ALT + T), в папке ostis/scripts выполним
* ./run_scweb.sh

После того, как выполнятся все команды, открываем браузер и переходим по ссылке «localhost:8000».
Если вы увидели стартовую страницу (узнаете из тысячи :) ) проекта по Истории г.Минска, то
### установка завершена успешно!



