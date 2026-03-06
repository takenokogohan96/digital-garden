---
{"dg-publish":true,"dg-permalink":"docker","permalink":"/docker/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-07T00:09:00.306+09:00"}
---

## インストールする
dockerdocs公式の [Install Docker Engine](https://docs.docker.com/engine/install/) に従う。ディストロによっても違う
## Dockerが起動していることを確認する
```
sudo systemctl status docker
```
## イメージとコンテナを表示する
```
# イメージ
docker images

# コンテナ
docker ps

# コンテナ（停止中含む）
docker ps -a
```
## イメージを取得する
```
# Docker Hub からDLする
docker pull ｛リポジトリ名｝
```
## イメージとコンテナを削除する
```
# コンテナ
docker rm {コンテナID}

# イメージ
docker rmi {イメージ名}
```
## Docker Compose で コンテナを起動する
1. あらかじめ `docker-compose.yml` を作成する
2. コマンドを入力する
```
# イメージを更新してコンテナを起動する
docker compose up --build

# バックグラウンドで起動する
docker compose up --build -d
```