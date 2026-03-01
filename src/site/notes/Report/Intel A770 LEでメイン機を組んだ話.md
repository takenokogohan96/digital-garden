---
{"dg-publish":true,"dg-permalink":"a770-machine-build","permalink":"/a770-machine-build/","tags":["Report"],"created":"2026-03-01T02:17:23.951+09:00","updated":"2026-03-01T18:40:04.557+09:00"}
---

2024年10月頃、Intel A770 Limited Edition を軸にメイン機を自作しました。
![a770le.jpg](/img/user/_img/Personal/a770le.jpg)
## 要件
1. Intel Arc A770 Limited Editionを使用すること
2. ”魅せる”PCとすること
    1. ケースのサイドパネルが透明であること
    2. 各パーツの色味が統一されていること（黒）
    3. アクスタなどを配置する余裕があること
3. サイズ感をITXとすること
4. 性能バランスが崩れない範囲で、型番に”7”を含むパーツを採用すること

## 調達したパーツ
![a770machine-parts.jpg](/img/user/_img/Personal/a770machine-parts.jpg)
### マザー：ASRock B760I Lightning WiFi
日本で手に入らないので米Amazonで輸入。
B760系かつITXかつ色が黒系で一番好みの見た目だった。

### CPU：Intel Core i7-12700K
当初non-kを予定していたが、在庫ないし上に値段がKとほぼ変化なしなのでK型番を選択。
F型番でないのは、dGPUとiGPUを連動させる「Intel Deep Link」機能なるものがあるから（尚、活かせていない模様）

### GPU：Intel Arc A770 Limited Edition
今回の主役。「リミテッドエディション」という響きが良いし、メーカ純正のロマンもある。
見た目もいい。アクスタとか置ける。

### メモリ：Crucial Pro DDR5-5600 16GB×2
個人的にメモリは Crucial に絶対的信用を寄せている。

### SSD：Western Digital SN770 1TB×2
型番に”7”がいっぱいあるし、登場時期的にも合うしグレード的にもちょうど良い。
片側がOSとソフトウェアインストール用で、もう片方が作業ストレージ用。

### 電源：SilverStone SX750 Gold
700~750WかつSFX電源かつ見た目が黒い安いのがこれだった。
ちなみに見た目のためだけに電源に張り付けられたシールは剥がした。

### ケース：DeepCool CH160
これがいいなと思っていたちょうどその頃に日本での発売を決定してくれました。感謝感激

### CPUファン：ID-COOLING IS-55
CPUファンは見た目重視のために背が低いトップフロー型を採用。

### ケースファン：ID-COOLINGの120mmを3つ
ケースファンと合わせメーカは ID-COOLING で統一。
## 組付けダイジェスト写真
### そり防止プレートとグリス
![a770machine-1.jpg](/img/user/_img/Personal/a770machine-1.jpg)
グリスは均一に塗る派。作業中にねじが行方不明になり三点止め
### CPUクーラー
![a770machine-2.jpg](/img/user/_img/Personal/a770machine-2.jpg)
120mmサイズのクーラーなのにマザーがITXなせいか巨大に見える
メモリの位置がクーラー直下なので、メモリ交換する場合はクーラー取り外し必須（面倒）
### ケース内への組付け
![a770machine-3.jpg](/img/user/_img/Personal/a770machine-3.jpg)
ギチギチ。ケースの仕様上ATX電源も選べるがGPUと干渉するためSFX電源を採用。
![a770machine-4.jpg](/img/user/_img/Personal/a770machine-4.jpg)
なんとか収まって組み立て完了
## 運用
![a770machine-5.jpg](/img/user/_img/Personal/a770machine-5.jpg)
CPUをTDP77W相当に設定してアイドル時40度、ピーク時75度程度の冷却度合を発揮。性能絞っても前メイン機（Ryzen 5 3600）よりベンチマークスコアが高くアーキテクチャの進化を感じた。

肝心の A770 は可もなく不可もなくといったところ。1440p環境のスタマスが快適だったので馬力はちゃんとありそうといった具合。

2030年くらいはまではこのA770マシンと過ごしたい。次の交換時には自作界隈もx86が淘汰されArmが台頭しているかも。