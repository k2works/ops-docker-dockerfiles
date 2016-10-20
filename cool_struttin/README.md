# cool_struttin

## 目的
Rubyアプリケーションベースイメージ

## 前提
| ソフトウェア     | バージョン    | 備考         |
|:---------------|:-------------|:------------|
| Ruby           | 2.3.1        |             |


## 構成
+ セットアップ
+ デプロイ

### セットアップ
```
$ vagrant up
$ vagrant ssh
$ cd /vagrant/cool_struttin
$ docker-compose build
$ docker-compose run ruby bash
$ ruby -v
$ exit
```

### デプロイ
```
$ vagrant up
$ vagrant ssh
$ cd /vagrant/cool_struttin
$ docker login
$ docker push harc/cool_struttin
```

