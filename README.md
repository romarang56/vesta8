Сборка VESTA 8
=============================

Установка
------------

1. Скачать и установить Drupal 8 (Позднее выложим сборку, со всеми необходимыми модулями)
2. git clone https://github.com/romarang56/vesta8.git
3. В папке с темой (./themes/vesta/) находим файл gulpfile.js
4. Редактируем строку  "let server_name = 'http://dp82.my';"
5. Запускаем gulp (Должен быть установлен npm!)

        $ npm -i 
        $ gulp 

Выключить дебаг
------------

Для выключения достаточно в файле ./sites/default/settings.php закомментировать строку

        if (file_exists($app_root . '/' . $site_path . '/settings.local.php')) {
            include $app_root . '/' . $site_path . '/settings.local.php';
        }
