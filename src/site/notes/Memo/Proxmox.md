---
{"dg-publish":true,"dg-permalink":"proxmox","permalink":"/proxmox/","tags":["Memo"],"created":"2026-03-01T02:17:20.400+09:00","updated":"2026-03-01T21:15:53.027+09:00"}
---

## CPU Governor
### 使用できる動作モードの一覧を表示
```
cat /sys/devices/system/cpu/cpu0/cpufreq/scaling_available_governors
```
### 現在の設定
```
cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
```
### 動作モードの変更（全コア）
```
echo "ondemand" | tee /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
```
### 動作モードを再起動後も反映する
1. `nano /etc/default/cpufrequtils`
2. 追記する `GOVERNOR="{動作モード}"`