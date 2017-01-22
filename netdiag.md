# Диагностика сетевых доступов
| Windows | Unix, MacOS - IPv4 |
| :----- | :---------------- |
| ipconfig /all | ifconfig -a |
| route print | netstat -rn |
| nslookup <хост> | host <хост> |
| nslookup <хост> 8.8.8.8 | host <хост> 8.8.8.8 |
| ping <хост>| ping -с 4 <хост> |
| tracert <хост> | traceroute -I <хост> |
| telnet <хост> <порт> | telnet <хоста> <порт> |

Каких-то из этих команд может не быть (telnet в Windows, обычно) - не сложно найти, как поставить. Номера портов можно найти здесь: https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers

Если вы подключены через vpn - выслать лог подключения, скорее всего ваш любимый поисковик в картинках покажет, как это сделать. Например, для OpenVPN, по запросу "openvpn client windows show connection logs" =) Кстати, в Windows openvpn клиент стоит попробовать запустить от администратора.
