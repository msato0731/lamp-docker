## 使い方
```
git clone https://github.com/uutarou10/lamp-docker-compose.git
cd lamp-docker-compose
```

### コンテナ起動・停止
コンテナ起動
```
docker-compose up -d
```

コンテナ停止
```
docker-compose stop
```

### コンテナへの接続
appコンテナへの接続
```
docker-compose exec app /bin/bash
```

dbコンテナへの接続
```
docker-compose exec db /bin/bash
```

### mysqlへの接続
mysqlへの接続
- Host: localhost
- Port: 13306
- Username: root
- Password: secret

```
mysql -u root localhost -P 3306 -p
```