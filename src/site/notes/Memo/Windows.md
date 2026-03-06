---
{"dg-publish":true,"dg-permalink":"windows","permalink":"/windows/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-07T00:08:57.521+09:00"}
---

## タスクバーの時刻に秒を表示
設定  > 時刻と言語 > 日付と時刻 > システムトレイに時刻と日付を表示する
![taskbarviewsecond.png](/img/user/_img/Tech/taskbarviewsecond.png)
## 定刻シャットダウン
1. トリガーの設定 > 実行間隔と時刻
2. 操作の編集
	1. プログラム/スクリプト：`shutdown`
	2. 引数：`-s -t 300 -c "表示文言"`

![taskscheduler-shutdown.jpg](/img/user/_img/Tech/taskscheduler-shutdown.jpg)
## Hyper-Vの入れ子
1. VMをシャットダウンしてホストOSに戻る
2. 以下のコマンドを投入
```
Set-VMProcessor –{仮想マシンの名前} -ExposeVirtualizationExtensions $true
```
