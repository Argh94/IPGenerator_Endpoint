# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-07 08:53:30 +0330

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
| 198.41.208.141 | 80, 443, 8080 | 51 |
| 190.93.247.15 | 80, 443, 8080 | 52 |
| 198.41.208.32 | 80, 443, 8080 | 52 |
| 198.41.215.246 | 80, 443, 8080 | 53 |
| 172.64.78.54 | 80, 443, 8080 | 53 |
| 172.67.98.38 | 80, 443, 8080 | 55 |
| 172.64.80.199 | 80, 443, 8080 | 57 |
| 172.64.86.122 | 80, 443, 8080 | 57 |
| 172.67.88.21 | 80, 443, 8080 | 57 |
| 172.67.141.130 | 80, 443, 8080 | 130 |
| 104.18.236.86 | 80, 443, 8080 | 136 |
| 104.17.139.26 | 80, 443, 8080 | 137 |
| 104.19.19.146 | 80, 443, 8080 | 138 |
| 104.17.91.74 | 80, 443, 8080 | 145 |
| 162.159.240.219 | 80, 443, 8080 | 145 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:90d6:9e9a:ab22:a26a:92e2:44d0] | 80, 443, 8080 | 3 |
| [2606:4700:c:a244:7d41:2060:9555:a205] | 80, 443, 8080 | 3 |
| [2606:4700:54:96a6:c4f1:d930:bd28:247d] | 80, 443, 8080 | 3 |
| [2606:4700:90d6:9e9a:ab22:a26a:92e2:44d0] | 80, 443, 8080 | 3 |
| [2606:4700:c:a244:7d41:2060:9555:a205] | 80, 443, 8080 | 3 |
| [2606:4700:54:96a6:c4f1:d930:bd28:247d] | 80, 443, 8080 | 3 |
| [2606:4700:90d6:9e9a:ab22:a26a:92e2:44d0] | 80, 443, 8080 | 3 |
| [2606:4700:c:a244:7d41:2060:9555:a205] | 80, 443, 8080 | 3 |
| [2606:4700:54:96a6:c4f1:d930:bd28:247d] | 80, 443, 8080 | 3 |
| [2606:4700:9c64:514c:23bb:3c40:4cdb:d85] | 80, 443, 8080 | 4 |
| [2606:4700:54:77f2:9f77:1b03:c2cc:cd86] | 80, 443, 8080 | 4 |
| [2606:4700:9c64:514c:23bb:3c40:4cdb:d85] | 80, 443, 8080 | 4 |
| [2606:4700:54:77f2:9f77:1b03:c2cc:cd86] | 80, 443, 8080 | 4 |
| [2606:4700:9c64:514c:23bb:3c40:4cdb:d85] | 80, 443, 8080 | 4 |
| [2606:4700:54:77f2:9f77:1b03:c2cc:cd86] | 80, 443, 8080 | 4 |

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
