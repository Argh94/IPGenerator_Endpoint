# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-13 10:24:00 +0330

## ✨ ویژگی‌ها
- 📡 **IPهای کم‌تأخیر**: مرتب‌شده بر اساس کمترین latency.
- 🔍 **پورت‌های پیشنهادی**: پورت‌های باز (80، 443، 8080) به‌صورت خودکار بررسی می‌شوند.
- ⏰ **به‌روزرسانی منظم**: هر ۵ ساعت با GitHub Actions.
- 📄 **خروجی‌های JSON**: داده‌ها در `list/ipv4.json`، `list/ipv6.json`، و `list/export.json` ذخیره می‌شوند.

## 📋 IPهای بهینه

**توجه:** پورت‌های نمایش‌داده‌شده توسط سرور بررسی شده‌اند، اما ممکن است بسته به شبکه شما متفاوت باشند. برای تأیید، از [YouGetSignal](https://www.yougetsignal.com/tools/open-ports/) (IPv4) یا [Nmap](https://nmap.org/) (IPv6) استفاده کنید.

### IPv4
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| 198.41.208.112 | 80, 443, 8080 | 50 |
| 172.64.88.212 | 80, 443, 8080 | 50 |
| 172.64.93.178 | 80, 443, 8080 | 51 |
| 162.159.251.225 | 80, 443, 8080 | 52 |
| 172.67.112.101 | 80, 443, 8080 | 59 |
| 173.245.49.128 | 80, 443, 8080 | 59 |
| 172.67.84.44 | 80, 443, 8080 | 59 |
| 198.41.222.166 | 80, 443, 8080 | 115 |
| 172.67.229.18 | 80, 443, 8080 | 131 |
| 172.67.231.30 | 80, 443, 8080 | 132 |
| 104.17.170.139 | 80, 443, 8080 | 134 |
| 104.17.232.39 | 80, 443, 8080 | 135 |
| 104.19.89.26 | 80, 443, 8080 | 136 |
| 104.17.127.135 | 80, 443, 8080 | 137 |
| 104.18.206.243 | 80, 443, 8080 | 141 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:3006:8e69:9df0:3027:2088:3af5] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:c5bd:c478:fa53:765a:8df] | 80, 443, 8080 | 3 |
| [2606:4700:3006:8e69:9df0:3027:2088:3af5] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:c5bd:c478:fa53:765a:8df] | 80, 443, 8080 | 3 |
| [2606:4700:3006:8e69:9df0:3027:2088:3af5] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:c5bd:c478:fa53:765a:8df] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:dfc2:eedb:aa43:bb0:63e4] | 80, 443, 8080 | 4 |
| [2606:4700:964d:eb7d:bed3:b2e0:e52:355e] | 80, 443, 8080 | 4 |
| [2606:4700:964d:f20c:808f:df18:ee52:a436] | 80, 443, 8080 | 4 |
| [2606:4700:8d7b:dfc2:eedb:aa43:bb0:63e4] | 80, 443, 8080 | 4 |
| [2606:4700:964d:eb7d:bed3:b2e0:e52:355e] | 80, 443, 8080 | 4 |
| [2606:4700:964d:f20c:808f:df18:ee52:a436] | 80, 443, 8080 | 4 |
| [2606:4700:8d7b:dfc2:eedb:aa43:bb0:63e4] | 80, 443, 8080 | 4 |
| [2606:4700:964d:eb7d:bed3:b2e0:e52:355e] | 80, 443, 8080 | 4 |
| [2606:4700:964d:f20c:808f:df18:ee52:a436] | 80, 443, 8080 | 4 |

## 🛠️ نصب و استفاده
1. **کلون کردن مخزن**:
   ```bash
   git clone https://github.com/Argh94/IPOptimizer.git
   ```
2. **تنظیمات PHP**:
   - PHP 8.0 یا بالاتر نصب کنید.
   - کلید API Hostmonit را در متغیر محیطی `HOSTMONIT_API_KEY` تنظیم کنید:
     ```bash
     export HOSTMONIT_API_KEY="your-api-key"
     ```
3. **اجرای اسکریپت**:
   ```bash
   php scripts/fetch_ips.php
   ```
4. **بررسی خروجی**:
   - فایل‌های JSON در پوشه `list/`.
   - لیست IPها در `README.md`.

## 📬 پشتیبانی
- 🐛 **گزارش مشکلات**: [Issues](https://github.com/Argh94/IPOptimizer/issues)
- 📧 **تماس**: [ircfspace@gmail.com](mailto:ircfspace@gmail.com)

## 📄 لایسنس
این پروژه تحت [لایسنس MIT](https://github.com/Argh94/HandWave/blob/main/LICENCE) منتشر شده است.
