Создание SSH ключа:
    $ ssh-keygen -t ed25519 -C "your_email@example.com"
    Игнорируем переименовку и пароли

    Активация (Добавление в агента):
        Запускаем агента
            $ eval "$(ssh-agent -s)"
        Добавляем свой ключ в активные (имя ключа может быть другим)
            $ ssh-add ~/.ssh/id_ed25519

Добавим в акккаунт на github
    Копируем содержимое публичного ключа (расширение .pub) и в настройках аккаунта добавляем новый ключ, сохраняем

Для копирования репозитория в нужную папку
    - Переходим в неё
    Вызываем команду:
        $ git clone <url>
        URL берём с сайта