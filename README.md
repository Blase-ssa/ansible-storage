# ansible-kafka
Ansible role for Kafka and Zookeeper 

Описание:
Пример ansible скриптов для автоматического масштабируемого развёртывания кластера для Kafka и zooKeeper.
Структура файлов набора выполнена согласно рекомендациям "alternative directory layout"
https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html#alternative-directory-layout

Перед использованием:
	- Заполните hosts файлы в директории inventory/dev (/test /prod)
	- В файле hosts не используйте алиасы, используйте имена которые можно использовать для разрешения имён ( это параметр используемый в скриптах)
	- Настройте авторизацию согласно имеющимся параметрам вашей инфраструктуры в файле inventory/dev (/test /prod)/group_vars bли host_vars если вам нужно использовать более индивидуальные настройки для каждого сервера
	- Настройте версию Kafka и zooKeeper


Как использовать:

Пример команды для запуска
ansible-playbook bootstrap.yml -i inventory/dev/hosts
