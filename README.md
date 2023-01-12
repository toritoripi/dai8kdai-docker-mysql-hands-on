# 第8課題　ハンズオンの実施

# 実施内容と結果報告
- コンテナの起動確認
```$ docker ps
CONTAINER ID   IMAGE                      COMMAND                  CREATED     STATUS          PORTS                               NAMES
278944e262f2   docker-mysql-hands-on-db   "docker-entrypoint.s…"   2 days ago  Up 46 seconds   33060/tcp, 0.0.0.0:3307->3306/tcp   docker-mysql-hands-on
```
- MySQLにログイン
```$ winpty docker compose exec db mysql -uroot -p
Enter password:
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 9
Server version: 8.0.31 MySQL Community Server - GPL
```
- movie_listがあることの確認
- moviesテーブルがあることの確認
- moviesテーブルのレコードの確認
![image](https://user-images.githubusercontent.com/114993632/212031591-2314a73f-c75c-4477-8d0e-bed09c0439e0.png)

- テーブルにレコードを追加する
- レコードの登録結果を確認する
![image](https://user-images.githubusercontent.com/114993632/212031961-7b914961-8943-4158-b7df-2d09b560e752.png)

- ログアウトする
- コンテナの停止
- 停止できていることの確認
![image](https://user-images.githubusercontent.com/114993632/212032312-295ac7d3-1eb3-4b6a-88c8-2b36ea2b2798.png)

# つまったところ
・Dockerのインストールはできたけどエラーがでていて起動できなかった。いろいろやってみたけど結局アンインストールしてやりなおした
・MySQLにログインするときパスワード入力ができなかった。表示されないだけでコンソールが認識しているから大丈夫とのことだった。
