---
{"dg-publish":true,"dg-permalink":"bios","permalink":"/bios/","tags":["Memo"],"created":"2026-03-01T04:50:16.000+09:00","updated":"2026-03-07T00:04:42.640+09:00"}
---



> [!NOTE] 確認環境
> マザーボード：[ASRock B760I Lightning WiFi](https://pg.asrock.com/mb/Intel/B760I%20Lightning%20WiFi/index.asp)
> CPU：[Intel Core i7-12700K](https://www.intel.com/content/www/us/en/products/sku/134594/intel-core-i712700k-processor-25m-cache-up-to-5-00-ghz/specifications.html)

## Intel CPU電力制限
1. BIOSを起動する
2. OCツール > CPU設定
	1. 長期間電力制限 > 平時使用の電力リミット（PL1）
	2. 短時間電力制限 > 高負荷時の電力リミット（PL2）

![Intelcpu-powerlimit.jpg](/img/user/_img/Tech/Intelcpu-powerlimit.jpg)
## RTCアラーム起動
1. BIOSを起動する
2. アドバンスド > ACPI設定 > RTC アラーム電源オン > 有効

![rtcalarm.jpg](/img/user/_img/Tech/rtcalarm.jpg)