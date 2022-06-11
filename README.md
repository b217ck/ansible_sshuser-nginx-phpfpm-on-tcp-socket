# ansible_sshuser-nginx-phpfpm-on-tcp-socket
Ansible роль для создания юзера с доступом по ssh, развертывания nginx и php-fpm по tcp socket

Разделите tasks на роли:
«Добавьте нового пользователя с авторизацией по ключу» — роль «users».
«Поднимите nginx server», «Укажите в nginx отправлять php на 9000 порт» — роль «http».
«Поднимите php-fpm», «Укажите php-fpm принимать на 9000 порт»— роль «php».

Поднимите nginx и php-fpm на разных серверах:
Для nginx сервера используйте роль «users» «http».
Для php-fpm сервера используйте роль «users» «php».
