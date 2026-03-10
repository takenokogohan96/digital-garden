---
{"dg-publish":true,"dg-permalink":"gnome","permalink":"/gnome/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-11T00:11:02.152+09:00"}
---

## Dockの機能を拡張する
1. Extension Manager を導入する
```
sudo apt install gnome-shell-extension-manager
```
1. [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/)を導入する
## トップバーの時計に秒を表示する
設定アプリ > システム > 日付と時刻 > 時計とカレンダー > 秒 を有効にする
![gnome-topber-displayseconds.png](/img/user/_img/Tech/gnome-topber-displayseconds.png)
## ログイン後にアクティビティ画面から開始しないようにする
1. Dash to Dock が導入されている
2. 拡張機能アプリ > Dash to Dock の設定 > 外観タブ と遷移する
3. 「Show overview on startup」を無効にする
![gnome-activitiesoverview.png](/img/user/_img/Tech/gnome-activitiesoverview.png)
## 画面拡大率を小刻にする
```
gsettings set org.gnome.mutter experimental-features '["scale-monitor-framebuffer", "xwayland-native-scaling"]'
```

## ファイラーに Google Drive を表示する
`gvfs-google` を導入する
https://archlinux.org/packages/extra/x86_64/gvfs-google/

> [!caution]
> ファイラー上ファイル名は正しく表示するが、別アプリ上では**ファイルID**を表示する
> ![gnome-gvfs-google-filer.png](/img/user/_img/Tech/gnome-gvfs-google-filer.png)
> ![gnome-gvfs-google-otherapps.png](/img/user/_img/Tech/gnome-gvfs-google-otherapps.png)


