# amadeus
Создание базы данных MySQL
Работаем в ОС Linux Ubuntu
Первый шаг загружаем через Терминал основные компоненты: Apache2, php, MySQL Server, phpMyAdmin
Чтобы установить MySQL сервер и phpMyAdmin на Ubuntu, выполните следующие шаги:

Обновляем список пакетов:

```sudo apt update```

Устанавливаем MySQL сервер:

```sudo apt install mysql-server```

После установки запускаем команду для настройки безопасности MySQL:

```sudo mysql_secure_installation```

Устанавливаем Apache2 веб-сервер:

```sudo apt install apache2```

Устанавливаем PHP и необходимые расширения:

```sudo apt install php libapache2-mod-php php-mysql```

Устанавливаем phpMyAdmin:

```sudo apt install phpmyadmin```

Во время установки будет предложено выбрать веб-сервер и настроить базу данных для phpMyAdmin. Выбераем Apache2 и настраиваем базу данных.
Подключаем phpMyAdmin к Apache:
Создаём символическую ссылку в каталоге Apache:

```sudo ln -s /usr/share/phpmyadmin /var/www/html/phpmyadmin```

Перезапускаем Apache:

```sudo systemctl restart apache2```

Теперь можем получить доступ к phpMyAdmin, перейдя по адресу http://ваш_сервер/phpmyadmin в нашем браузере.

Следующие шаги:

Настройка брандмауэра для защиты сервера.
Создание пользователей и баз данных в MySQL.
