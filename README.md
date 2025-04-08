# IFMO_DistributedComputing_for_DevOps
Distributed Computing course for DevOps 2025

Требования:
- установленный ansible на хост-машине
- ОС Ubuntu и установленный openssh на сервере(-ах), куда будет устанавливаться wordpress

Инструкция:
1. Изменить файл `wordpress/inventory/hosts`, где надо указать свой сервер
2. Применить `ansible-playbook -i inventory/hosts site.yml`