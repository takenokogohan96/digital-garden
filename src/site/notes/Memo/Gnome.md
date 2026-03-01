---
{"dg-publish":true,"dg-permalink":"gnome","permalink":"/gnome/","tags":["Memo"],"created":"2026-03-01T02:17:20.348+09:00","updated":"2026-03-01T19:18:04.311+09:00"}
---

## Dash to Dockを導入する
Gnome Shell Extensionsを介する
https://extensions.gnome.org/extension/307/dash-to-dock/
## トップバーの時計に秒を表示する
設定アプリ > システム > 日付と時刻 > 時計とカレンダー > 秒 を有効にする
![gnome-topber-displayseconds.png](/img/user/_img/Tech/gnome-topber-displayseconds.png)
## ログイン後にアクティビティ画面から開始しないようにする
1. Dash to Dock が導入されている
2. 拡張機能アプリ > Dash to Dock の設定 > 外観タブ と遷移する
3. 「Show overview on startup」を無効にする
![gnome-activitiesoverview.png](/img/user/_img/Tech/gnome-activitiesoverview.png)
## 画面拡大率の小刻にする
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


