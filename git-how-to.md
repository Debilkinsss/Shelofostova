Сначала заполняем данные о пользователе в терминале при помощи команд:
git config --global user.email "nselofostova@gmail.com"
git config --global user.name "Шелофостова Анастасия"
Создаем ключ при помощи комнады, открываем его в Вижуал Студио Код, копируем и вставляем в "добавить ключ SSH":
ssh-keygen -t ed25519 -C "nselofostova@gmail.com"
Потом при помощи агента создать ещё приватный ключ:
eval "ssh-agent -s"
ssh-add ~/.ssh/id_ed25519
Таке при помощи команды мы клонируем репозиторий на локальный компьютер:
git clone git@github.com:Debilkinsss/Shelofostova.git
