# Что это и для чего?
Это небольшой скрипт для поиска номера звонившего на вашу IP ATC Asterisk. Написанный на PHP 8.1
----------
Для чего, придумайте сами :)
# О скрипте
В скрипте есть небольшая админка, чёрный список, счётчик звонков, скачивание аудио в формате .wav
![image](https://github.com/zavsc/asterisk/assets/90477403/8794eae4-7c82-4b11-90b5-4c3c5050fc00)
![image](https://github.com/zavsc/asterisk/assets/90477403/588e6107-55aa-42ec-b7d9-2521ca912fa3)
# Как установить?
Установка производится на сервер ATC Asterisk.
----------
Закидываете файлы и в admin.php и index.php, меняете пути где лежат ваши записи с /var/lib/asterisk/records на ваш путь.
----------
Меняете в admin.php при желании стандартный пароль (admin) на 4-ой строке: $adm = 'admin';
----------
Чёрный список настраивается в index.php (это те номера которые не будут видны без админки) на 3-ей строке:
$ban_list = array('7777777777','7766466468');
----------
На этом установка окончена.
