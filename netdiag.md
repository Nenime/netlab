# Диагностика сетевых проблем
1. При подключении через OpenVPN
 - (для Windows) запустить клиент OpenVPN от имени администратора
 - собрать лог подключения
 
2. В консоли необходимо выполнить и собрать результаты (в Windows консоли тоже можно выделять текст):

 | Windows | Unix, MacOS - IPv4 |
 | :----- | :---------------- |
 | ipconfig /all | ifconfig -a |
 | route print | netstat -rn |
 | nslookup <хост> | host <хост> |
 | nslookup <хост> 8.8.8.8 | host <хост> 8.8.8.8 |
 | ping <хост>| ping -с 4 <хост> |
 | tracert <хост> | traceroute -I <хост> |
 | telnet <хост> <порт> | telnet <хоста> <порт> |

 Каких-то из этих команд может не быть по-умолчанию (telnet в Windows, обычно). Номера портов можно найти здесь: https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers