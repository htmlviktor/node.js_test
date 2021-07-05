# node.js_test

Описание: Сделать сервис с REST API. Авторизация по bearer токену (/info, /latency, /logout). Настроенный CORS для доступа с любого домена. DB - MongoDB (или реляционная БД, на усмотрение разработчика). Токен действителен 1 час. 

API:

/signin [POST] - запрос bearer токена по id и паролю // данные принимает в json
/signup [POST] - регистрация нового пользователя: // данные принимает в json
Поля id и password, id - номер телефона или email. После регистрации пометить в профиле тип id (phone/mail)
При удачной регистрации вернуть bearer токен.
/info [GET] - возвращает id пользователя и тип id.
/latency [GET] - возвращает задержку от сервиса до google.com
/logout [GET] - с паметром all:
true - удаляет все bearer токены пользователя
false - удаляет только текущий bearer токен

# Дополнительно

Написать front-end часть приложения на React.js, которая будет отображать пользователя и информацию о нём. 


# Деплой

Задеплоить на Heroku или любой другой бесплатный сервис для Node.js окружения. Если есть front-end деплоить на Vercel или любой другой доступный сервис. 


# Контроль версий

Код приложения стоит поместить в гитхаб и предоставить ссылку на код(репозиторий) и опубликованную версию проекта. 
