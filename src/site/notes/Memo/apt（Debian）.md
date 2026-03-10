---
{"dg-publish":true,"dg-permalink":"ubuntu","permalink":"/ubuntu/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-07T00:08:58.444+09:00"}
---

## aptコマンド
### パッケージリストを更新する
```
sudo apt update
```
### 全てのパッケージを更新する
```
# オプションなし
sudo apt upgrade

# y/nをyで自動的に進める
sudo apt upgrade -y
```
### パッケージをインストールする
```
sudo apt install {パッケージ名}
sudo apt install {パッケージ名} -y
```
### インストール済みのパッケージ名を表示する
```
# 全部
apt list --installed

# 特定のパッケージ名（なければ表示なし。あれば[installed]）
apt list --installed ｛パッケージ名｝
```
### パッケージをアンインストールする
```
sudo apt remove {パッケージ名}
sudo apt remove {パッケージ名} -y
```
