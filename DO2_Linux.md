## Part 1. Инструмент ipcalc



### 1.2. localhost

Можно обратиться к приложению с IP: 
127.0.0.2/24
127.1.0.1/8

Нельзя обратиться к приложению с IP:
194.34.23.100
128.0.0.1

### 1.3. Диапазоны и сегменты сетей

какие из перечисленных IP можно использовать в качестве публичного, а какие только в качестве частных:

10.0.0.45 - частный
134.43.0.2 - публичный
192.168.4.2 - частный
172.20.250.4 - частный
172.0.2.1 - публичный
192.172.0.1 - публичный
172.68.0.2 - публичный
172.16.255.255 - частный
10.10.10.10 - частный
192.169.168.1 - публичный

какие из перечисленных IP адресов шлюза возможны у сети 10.10.0.0/18:

10.0.0.1 - не подходит
10.10.0.2 - возможен
10.10.10.10 - возможен
10.10.100.1 - не подходит
10.10.1.255 - возможен

## Part 2. Статическая маршрутизация между двумя машинами

## Part 3. Утилита iperf3

3.1. Скорость соединения

Перевести и записать в отчёт:

8 Mbps = 1 MB/s(мегабит/c в мегабайт/c)

100 MB/s = 819200 Kbps(мегабайт/c в килобит/c)

1 Gbps = 1024 Mbps(гигабит/c в мегабит/c)


### 5.4. Добавление статических маршрутов

Для адреса 10.10.0.0/18 был выбран маршрут, отличный от 0.0.0.0/0, потому что при наличии нескольких маршрутов одинаковой длины выбирается тот маршрут, который задан наиболее точно.

### 5.5. Построение списка маршрутизаторов

Утилита Traceroute вместо ICMP-запроса отправляет 3 UDP-пакета на определенный порт целевого хоста и ожидает ответа о недоступности этого порта. Первый пакет отправляется с TTL=1, второй с TTL=2 и так далее, пока запрос не попадёт адресату. Так как вместо ICMP-запроса он отправляет UDP-запрос, в каждом запросе есть порт отправителя и порт получателя. По умолчанию запрос отправляется на закрытый порт 34434. Когда запрос попадёт на хост назначения, этот хост отправит ответ о недоступности порта «Destination port unreachable» (порт назначения недоступен). Это значит, что адресат получил запрос. Traceroute воспримет этот ответ как завершение трассировки.

### 5.6. Использование протокола ICMP при маршрутизации

## Part 6. Динамическая настройка IP с помощью DHCP

