Vector-role
=========

Роль устанавливает Vector.

Требования к окружению
------------

rpm-based дистрибутив Linux (CentOS, RedHat).

Установленные пакеты:
- git
- wget
- curl
- unzip
- gnupg
- nginx

Переменные роли
--------------
```YAML
#Версия пакета Vector
vector_version: 0.22.0
```

Зависимости
------------

Нет

Пример playbook
----------------
```YAML
- name: Install vector
  hosts: vector
  become: yes
  become_user: root
  remote_user: vagrant
  roles:
    - vector
  tags: vector
```
License
-------

Free

Информация об авторе
------------------

Реализация: Дмитрий Багрянский
