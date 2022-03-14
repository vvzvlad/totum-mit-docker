### Если вы хотите быстро посмотреть

Если у вас установлены Docker, Docker-compose и Git  и вы хотите попробовать, то:

— клонируете репозитарий docker-установки;

— назначаете 777 всем папкам и 666 всем файлам, тк контейнеры работает от пользователя uid 201608:201608 и 201609:201609

```
git clone https://github.com/totumonline/totum-mit-docker.git && cd totum-mit-docker && sudo find . -type d -exec chmod 777 {} \; && sudo find . -type f -exec chmod 666 {} \;
```



Стартуете Docker-compose:

```
docker-compose up -d
```



Открываем браузер на localhost, выбираем язык установки и заполняем в разделе Создать суперпользователя Тотум:

— пароль, который будет использован для суперпользователя Totum

— ваш Email для Cron-нотификаций (никуда не отправляется, будет записан в конфиг)

— заполнив наживаем Создать конфиг и залить схему

**Ждем, переходим по ссылке, готово!**



#### Если у вас установлен Docker и вы хотите сконфигурировать полностью — [посмотрите эту инструкцию](https://github.com/totumonline/totum-mit-docker/blob/main/IF_YOU_ALREADY_HAVE_DOCKER_RU.md)



#### Если вам нужно сконфигурировать чистую систему — [посмотрите эту инструкцию для ubuntu](https://github.com/totumonline/totum-mit-docker/blob/main/FULL_CONFIG_ON_CLEAR_UBUNTU_RU.md)