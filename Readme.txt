1) Установил Clickhouse
2) Включил доступ к нему по сети
3) Добавил конфиг monitoring.xml в каталог /etc/clickhouse/config.d/
4) Перезапустил Clickhouse
5) Проверил доступность метрик (curl http://127.0.0.1:9363/metrics), получил ответ (см рисунок 1)
6) Установил Prometheus на отдельную ВМ
7) Добавил Clickhouse в конфиг Prometheus
8) Перезапусил Prometheus. В Target'ах увидел подключение к Clickhouse по порту 9363 (см рисунок 2)
9) Установил Grafana, подключил ее к Prometheus. 
10) Добавил дашборд для встроенного экспортера Clickhouse (см рисунок 3)
