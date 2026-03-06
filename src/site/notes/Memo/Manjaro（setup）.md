---
{"dg-publish":true,"dg-permalink":"manjaro","permalink":"/manjaro/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-07T00:04:42.642+09:00"}
---


## 豆腐を消す
### 日本語
```
sudo pacman -S otf-ipafont
```
投入後再起動する

### Emoji
```
sudo pacman -S noto-fonts-emoji unicode-emoji nodejs-emojione
```
投入後再起動する

### 韓国語
```
sudo pacman -S noto-fonts-cjk
```
投入後再起動する


## 日本語入力環境を整える
### Fictx5本体を導入する
```
sudo pacman -S manjaro-asian-input-support-fcitx5
```
Gnome環境の場合、加えてGnome拡張 [Input Method Panel](https://extensions.gnome.org/extension/261/kimpanel/) を入れる
- 変換候補のポップアップ表示位置を入力入力と被らせない
- IMEの状態(MozcなJP⇔US など)をトップバーに表示する
### カタカナ英語の変換
[カナ英辞書v2.txt](https://www.mediafire.com/?cy1mxpjds5l5h)を辞書ツールに導入する
![fcitx5-kana-english.png](/img/user/_img/Tech/fcitx5-kana-english.png)
## アイコン（papirus）
アイコン：[papirus-icon-theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)
フォルダー（色指定）：[papirus-folders](https://github.com/PapirusDevelopmentTeam/papirus-folders)

## スワップ領域の作成
[ArchWiki の Swap](https://wiki.archlinux.org/title/Swap#Swap_file) に従いスワップ領域を削除してから再作成を行う。
> [!NOTE]
> 新規にManjaroをインストールしたさいスワップファイル作成する設定にしても、数百MB程度しかスワップ領域が確保されない場合がある。

## Fastfetch
![fastfetch.png](/img/user/_img/Tech/fastfetch.png)
> [!caution]
> かつての `Neofetch` は開発が終了している。