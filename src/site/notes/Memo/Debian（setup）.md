---
{"dg-publish":true,"dg-permalink":"debian","permalink":"/debian/","tags":["Memo"],"created":"2026-03-08T22:11:04.489+09:00","updated":"2026-03-11T01:35:09.356+09:00"}
---

> [!NOTE] 構築環境
> Model：ThinkPad X1 Nano Gen1
> OS：Debian GNU/Linux 13(trixie)
> DE：Gnome
## OSのインストール
1. [公式HP](https://www.debian.org)からisoファイルをDLする
2. [Rufus](https://rufus.ie)でインストールメディアを作成する
3. インストール、初回セットアップを完了する
## OSのチューニング
### 自ユーザにsudo権限を付与する
Rootユーザーに切り替える
```
su -
```
自ユーザーをsudoグループに追加する 
```
usermod -aG sudo {自ユーザ名}
```
再起動する（設定を反映する）
```
reboot
```
### ターミナルをZshに入れ替える
Zshをインストールする
```
sudo apt install zsh
```
oh my zsh（構成ツール）をインストールする
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
Powerlevel10k テーマをダウンロードする
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
Powerlevel10k テーマ推奨フォントをターミナルに設定する
- github > [Meslo Nerd Font patched for Powerlevel10k](### Meslo Nerd Font patched for Powerlevel10k)
- インストール後、ターミナルでフォント設定する

Powerlevel10k テーマ を設定する
- `~/.zshrc` を nano で開く
- 上書きする `ZSH_THEME="powerlevel10k/powerlevel10k"`
- 再起動し、設定ウィザードに従う

### Gnome の表示周りを調整する
別メモ [[Memo/Gnome\|Gnome]] を参照
## ソフト導入基盤を整える
### Flatpak/hubをセットアップする
公式の[Debian向けセットアップガイド](https://flathub.org/ja/setup/Debian)を参照する
### Firefox Developer Editionをセットアップする
公式の[Linux向けインストールガイド](https://support.mozilla.org/ja/kb/install-firefox-linux)の「Debian ベースのディストリビューションに Firefox の .deb パッケージをインストールする (推奨)」を参照する
### Progressive Web Apps for Firefox をセットアップする
 [公式アドオンストア](https://addons.mozilla.org/ja/firefox/addon/pwas-for-firefox/)から導入する
> [!caution]
> flatpak版firefoxではインストールが進行しなかっため。多分 .deb パッケージ版が必要。
## 必要なソフトを導入する

| 導入方法                  | 使い分け                    |
| --------------------- | ----------------------- |
| **apt** / **Flatpak** | - ストアにある                |
| **PWA**<br>           | - ストアにない<br>- Web版で足りる  |
| **Native**            | - ストアにない<br>- Web版で足りない |
