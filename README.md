1C-RAS Prometheus data exporter
========
Ещё один экспортер метрик для Prometheus с 1C-RAS, не требующий установки 1C-RAC.
Экспортер работает в двух режимах push и pull.
Для работы в режиме push требуется pushgateway в таргетах Prometheus. 
На текущий момент экспортируются показатели запущеных rpHosts.

Demo
========
### Склонируйте репозиторий, отредактируйте файл .env:
```
git clone https://github.com/Chipazawra/v8-1c-cluster-pde
```
### Содержимое ./.env:
```
RAS_HOST=<ras host>
RAS_PORT=<ras port>
CLS_USER=<ras user - если есть>
CLS_PASS=<ras pass - если есть>
```
### Запустите docker-compose:
```
docker-compose up
```

### Результатом проделанных действий на `http://<host-ip>:3000` или есть вы делали это на своей машине `http://localhost:3000` будет доступна Grafana c demo дабордом:

![image](https://user-images.githubusercontent.com/18016416/147658562-322a2f01-61d7-496a-a256-57d11ae6beae.png)

