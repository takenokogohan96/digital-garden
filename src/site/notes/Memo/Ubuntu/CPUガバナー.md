---
{"dg-publish":true,"dg-permalink":"cpu-governor","permalink":"/cpu-governor/","created":"2026-02-15T13:20:43.076+09:00","updated":"2026-02-15T13:26:19.780+09:00"}
---

使用できる動作モードの一覧を表示
```
cat /sys/devices/system/cpu/cpu0/cpufreq/scaling_available_governors
```
現在の設定
```
cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
```
動作モードの変更（全コア）
```
echo "ondemand" | tee /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
```
動作モードを再起動後も反映する
1. `nano /etc/default/cpufrequtils`
2. 追記する `GOVERNOR="{動作モード}"`