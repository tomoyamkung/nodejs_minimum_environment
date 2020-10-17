# nodejs_minimum_environment

Node.js を環境へインストールせずに実行するためだけのプロジェクト。

ビルド：

```sh
$ docker-compose up -d
```

以下はコマンド例。

例：src/helloworld.js を実行する：

```sh
$ docker-compose run --rm app node helloworld.js
Hello World!
```

例：コンテナに入って、Node.js のバージョンを確認する：

```sh
$ docker exec -it NODEJS_MINIMUM_CONTAINER_NAME bash
root@92478d7f50a5:/src# node --version
v12.19.0
```
