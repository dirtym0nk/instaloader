# instaloader

Это подробное описание для тех, кто хочет сделать резервную локальную копию своего instagram.
Для того, чтобы скачать посты, актуальное и описание со своего профиля, вам понадобится компьютер и интернет.

Шаги:
1) Необходимо установить на свой пк язык программирования python. Для этого перейдите по ссылке (https://www.python.org), наведеите курсор на download и скачайте установочный файл. Установите python.
2) Создайте папку не очень глубоко в файловой системе.
3) Необходимо открыть терминал (командную строку). На windows это можно сделать, введя в поисковую строку рядом с пуском "cmd". На mac - открыть терминал через spotlight.
4) Используя команды для навигации в терминале, перейдите в созданную заранее папку. Посмотреть команды можно тут https://ru.hexlet.io/courses/cli-basics/lessons/navigation/theory_unit. Основые - это cd, ls, pdw.
5) Находясь в нужной папке, нужно создать виртуальное окружение, чтобы не захламлять файловую систему. 
Введите команду (python3 -m venv venv) без скобок.
Введите ls, должна появиться папка venv.
6) Активируем виртуальное окружение командой (. ./venv/bin/activate)
7) Установим библиотеки для скачивания ваших фото и видео командой (pip install instaloader).
8) Необходимо произвести вход в вашу учетную запись instagram. Для этого введите (instaloader --login название вашего профиля)
к примеру instaloader --login alexey_paluchaetsa. Жмем "ввод".
9) Ведите пароль от инстаграмма.
10) Дальше все просто) введите следущую команду с названием своего профиля вместо моего.
      'instaloader --login alexey_paluchaetsa alexey_paluchaetsa --no-metadata-json --no-profile-pic -profile'
11) В созданной папке появится новая папка, в которую скачаются все посты с вашей страницы.
12) Для того чтобы скачать актуальное, введите команду, заменив название моего профиля на свой.
      instaloader --login alexey_paluchaetsa alexey_paluchaetsa --no-metadata-json --no-posts --no-profile-pic --highlights -profile
