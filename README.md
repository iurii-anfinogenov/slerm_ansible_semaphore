# slerm_ansible_semaphore
Плейбук для практикума по ansible, школа ["Слёрм"](https://slurm.io/)  
Для работы плейбука требуется:
- Установлен ansible
- Установлена [роль](https://github.com/geerlingguy/ansible-role-postgresql) для postgresql командой: `ansible-galaxy role install geerlingguy.postgresql`
- Сервер (вм) ОС Ubuntu с пользователем добавленым в группу sudo
- Данные (IP-адрес, Логин, Пароль) добавлены в файл hosts.ini

После установки сервис доступен `<ip-address>:3000`  
Поменять пароль можно командой на сервере: 
```shell
semaphore user change-by-login --login admin --password admin
```