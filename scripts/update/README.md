## Новый метод деплоя

Если для вашего кода необходимо выполнить определенные действия, например:

```sh
drush en -y mymodule
```

Вам надо в эту папку положить файл в формате `issue-[#number].sh`:
```sh
#!/bin/sh

drush -y en mymodule
```

Скрипт будет вызван из папки: "$HOME/domains/$SETTINGS_DOMAIN"
