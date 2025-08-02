# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-02 04:37:08 +0330

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
| 172.67.121.163 | 80, 443, 8080 | 45 |
| 172.67.68.79 | 80, 443, 8080 | 47 |
| 172.67.140.38 | 80, 443, 8080 | 130 |
| 172.67.168.68 | 80, 443, 8080 | 130 |
| 172.67.161.62 | 80, 443, 8080 | 131 |
| 104.18.162.35 | 80, 443, 8080 | 132 |
| 104.17.248.11 | 80, 443, 8080 | 132 |
| 104.18.162.35 | 80, 443, 8080 | 132 |
| 104.17.248.11 | 80, 443, 8080 | 132 |
| 104.19.215.181 | 80, 443, 8080 | 133 |
| 104.19.230.168 | 80, 443, 8080 | 133 |
| 104.19.215.181 | 80, 443, 8080 | 133 |
| 104.19.230.168 | 80, 443, 8080 | 133 |
| 104.18.183.117 | 80, 443, 8080 | 135 |
| 104.18.183.117 | 80, 443, 8080 | 135 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:99ef:43d5:ab98:883d:bc4c:6c8e] | 80, 443, 8080 | 3 |
| [2606:4700:9b0b:2221:3965:c2a5:3c9d:b576] | 80, 443, 8080 | 3 |
| [2606:4700:9b0f:fc76:db6d:9b9a:dbea:82be] | 80, 443, 8080 | 3 |
| [2606:4700:99ef:43d5:ab98:883d:bc4c:6c8e] | 80, 443, 8080 | 3 |
| [2606:4700:9b0b:2221:3965:c2a5:3c9d:b576] | 80, 443, 8080 | 3 |
| [2606:4700:9b0f:fc76:db6d:9b9a:dbea:82be] | 80, 443, 8080 | 3 |
| [2606:4700:99ef:43d5:ab98:883d:bc4c:6c8e] | 80, 443, 8080 | 3 |
| [2606:4700:9b0b:2221:3965:c2a5:3c9d:b576] | 80, 443, 8080 | 3 |
| [2606:4700:9b0f:fc76:db6d:9b9a:dbea:82be] | 80, 443, 8080 | 3 |
| [2606:4700:99ec:5032:2af0:4b90:a8f6:7784] | 80, 443, 8080 | 4 |
| [2606:4700:9b0f:d195:abda:79f0:38de:f3fe] | 80, 443, 8080 | 4 |
| [2606:4700:99ec:5032:2af0:4b90:a8f6:7784] | 80, 443, 8080 | 4 |
| [2606:4700:9b0f:d195:abda:79f0:38de:f3fe] | 80, 443, 8080 | 4 |
| [2606:4700:99ec:5032:2af0:4b90:a8f6:7784] | 80, 443, 8080 | 4 |
| [2606:4700:9b0f:d195:abda:79f0:38de:f3fe] | 80, 443, 8080 | 4 |

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
