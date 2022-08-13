# 実行コマンド
```
docker-compose up --build
```

---

# コンテナ操作

## app内
コンテナに入るコマンド
```
docker-compose exec -it app bash
```

---

## mysql内
コンテナに入るコマンド
```
docker-compose exec -it mysql bash
```

mysqlの中に入る
```
# ユーザーを設定してmysqlに入る。次にパスワード入力が要求される
mysql -u user -p

# ワンライナーで入りたい場合（セキュリティには十分ご注意ください。）
mysql -u user -p'yourStrong(!)Password'
mysql -u user --password='yourStrong(!)Password'
```