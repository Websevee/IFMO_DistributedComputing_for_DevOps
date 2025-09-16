# IFMO_DistributedComputing_for_DevOps
Distributed Computing course for DevOps 2025

Требования:
- установленный ansible на хост-машине
- ОС Ubuntu и установленный openssh на сервере(-ах), куда будет устанавливаться wordpress

Инструкция:
1. Изменить файл `wordpress/inventory/hosts.yml`, где надо указать свой сервер
2. Применить `ansible-playbook -i inventory/hosts.yml playbook1.yml`
3. Применить `ansible-playbook -i inventory/hosts.yml playbook2.yml`
4.1. Изменить в `group_vars/monitoring` значение ключа `grafana_api_key` на созданный вами API KEY в Grafana.Необходимо для авторизации
4.2. Применить `ansible-playbook -i inventory/hosts.yml playbook3.yml`
5. Если все сработало - будет доступно по адресу `[ip]:80` (в базовом примере, `http://192.168.88.126:80/`)

![image](https://github.com/user-attachments/assets/ddccd044-52bc-41f0-9bb3-2817c7f48640)
