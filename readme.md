# docker-centos7-nodebrew

nodebrewをインストールしたCentOS7のDockerfileです。

## イメージをビルドをするコマンドサンプル

NODE_VERSION にはインストールするNode.jsのバージョンを指定します。

指定しない場合最新の安定版がインストールされます。

```
$ docker build --tag nodebrew --build-arg NODE_VERSION=v8.10.0 ./docker-centos7-nodebrew
```

## コンテナを作成するコマンドサンプル

```
$ docker run -it -d --name nodebrew -p 3000:3000 -v ~/src:/root/src nodebrew /bin/bash
```

## コンテナを起動するコマンド

```
$ docker start nodebrew
```

## コンテナを終了するコマンド

```
$ docker stop nodebrew
```
