# linux-forensics

Для Linux информация хранится в файлах по различным путям.

/etc/os-release - файл с инф. о выпуске ОС
/etc/passwd     - инф. об УЗ пользователей. Вывод содержит 7 полей разделенные ':'
- регистрационное имя или логин;
- хеш пароля (x) информация о хеш пароля хранится в etc/shadow.
- идентификатор пользователя;
- идентификатор группы по умолчанию;
- описание УЗ;
- домашний каталог УЗ;
- регистрационная оболочка, или shell.

/etc/group 	- инф. о группах пользователей.
/etc/sudoers 	- список sudoers, linux пользволяет повышать привилегии до sudo, которые присутствуют в этом файле.

/var/log - журналы всех видов.
/var/log/btmp - инф. о неудачных входах в систему;
/var/log/wtmp - инф. о входах в систему.

/var/log/auth.log - журнал аутентификации. ("time Hostname sudo: username" - пример повышения привилегии из журнала).

/etc/hostname	- имя хоста;
/etc/timezone	- часовой пояс;

/etc/network/interfaces	- информация о сетевых интерфейсах;
ip - утилита для информации о MAC и IP-адресах интерфейсов, только для "живых" систем.
netstat - утилита, поиска активных сетевых подключений. смотреть man по утилите.
ps - информация о запущенных процессах.
/etc/hosts - конфигурация для значения имени DNS.
/etc/resolv.conf - инф. о DNS-серверах с которыми общается Linux для разрешения DNS.

Закрепление:

cron - планировщик заданий.
/etc/crontab - список заданий.
/etc/init.d - каталог со списом служб.
.bashrc - когда запускается оболочка bash, она запускает команды в .bashrc.
/etc/bash.bashrc
/etc/profile

Доказательства выполнения:
/var/log/auth.log - информация и запуске с SUDO.
~/.bash_history - для каждой УЗ хранится в домашнем каталоге УЗ.
~/.viminfo - инф. открытых файлов в vim.

