# Synology 7 — доступ с правами root для WinSCP
1.	Включить в панели управления DSM доступ по SSH (22 порт по умолчанию)
2.	С помощью Putty войти в систему с правами 
3.	Ввести команду
- sudo -i 
	еще раз ввести пароль от учетной записи
5.	Ввести команду 
- synouser --setpw root (пароль для root)
5.	Ввести команду
- vi /etc/ssh/sshd_config
6.	редоктирование SHIFT+I потом ESC.
7.	Найти текст 
   #PermitRootLogin yes, убрать #, тем самым разрешив доступ с правами root
8.	Нажать Esc , затем вести :wq!, нажать Enter
9.	Нажать Esc , затем вести :q!
10.	Ввести команду reboot
