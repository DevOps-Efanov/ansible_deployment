## Описание

Проект предназначен для автоматизированного развертывания MariaDB, Prometheus, Grafana и необходимых экспортеров с использованием Ansible. Он включает в себя настройку фаервола для обеспечения безопасности.

## Структура проекта

- ansible.cfg — конфигурационный файл Ansible.
- hosts — инвентарный файл для Ansible.
- playbook.yml — основной playbook для развертывания.
- roles/ — директория с ролями для установки MariaDB, Prometheus, Grafana и настройки фаервола.

## Установка и запуск

1. Клонируйте репозиторий:
   
   git clone https://github.com/DevOps-Efanov/ansible_deployment.git

   cd ansible_deployment

2. Настройте файл hosts, указав IP-адреса серверов.

3. Запустите playbook:
   
   ansible-playbook -i hosts playbook.yml --ask-become-pass
   
