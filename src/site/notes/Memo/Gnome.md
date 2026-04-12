---
{"dg-publish":true,"dg-permalink":"gnome","permalink":"/gnome/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-12T00:05:59.312+09:00"}
---

## Settings
### 画面拡大率を小刻にする
```
gsettings set org.gnome.mutter experimental-features '["scale-monitor-framebuffer", "xwayland-native-scaling"]'
```
- トップバーの時計に秒を表示する
	- 設定アプリ > システム > 日付と時刻 > 時計とカレンダー > 秒 を有効にする

## Extension Manager
```
sudo apt install gnome-shell-extension-manager
```
-  [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/) - Dockの見た目、挙動をカスタマイズする
	- ログイン後にアクティビティ画面から開始しないようにする
		- 「Show overview on startup」を無効にする
-  [Input Method Panel](https://extensions.gnome.org/extension/261/kimpanel/) - トップバーにIMEの状態を表示する
## Tweaks
```
sudo apt install gnome-tweaks
```
- [Vimix-cursors](https://github.com/vinceliuice/Vimix-cursors) - カーソル
- [Papirus](https://github.com/PapirusDevelopmentTeam/papirus-folders) - アイコン
- [Papirus Folders](https://github.com/PapirusDevelopmentTeam/papirus-folders) - フォルダアイコン
## Grub（Grub Customizer）
```
sudo apt install grub-customizer
```
- [Distro Grub Themes](https://github.com/AdisonCavani/distro-grub-themes?tab=readme-ov-file) - ディストロテーマ
## plymouth-themes
- [Linux Distro Logos](https://www.pling.com/p/2106821) - ディストロテーマ
## ファイラーに Google Drive を表示する
`gvfs-google` を導入する
https://archlinux.org/packages/extra/x86_64/gvfs-google/

> [!caution]
> ファイラー上ファイル名は正しく表示するが、別アプリ上では**ファイルID**を表示する
> ![gnome-gvfs-google-filer.png](/img/user/_img/gnome-gvfs-google-filer.png)
> ![gnome-gvfs-google-otherapps.png](/img/user/_img/gnome-gvfs-google-otherapps.png)


