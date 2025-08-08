# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-08 08:53:27 +0330

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
| 198.41.208.186 | 80, 443, 8080 | 50 |
| 198.41.215.41 | 80, 443, 8080 | 56 |
| 172.67.95.127 | 80, 443, 8080 | 56 |
| 162.159.255.114 | 80, 443, 8080 | 56 |
| 172.67.70.123 | 80, 443, 8080 | 57 |
| 172.67.202.113 | 80, 443, 8080 | 131 |
| 104.18.106.37 | 80, 443, 8080 | 135 |
| 104.17.134.19 | 80, 443, 8080 | 136 |
| 104.19.197.11 | 80, 443, 8080 | 137 |
| 104.16.173.208 | 80, 443, 8080 | 138 |
| 162.159.248.42 | 80, 443, 8080 | 142 |
| 162.159.255.57 | 80, 443, 8080 | 217 |
| 172.67.193.216 | 80, 443, 8080 | 225 |
| 172.67.233.163 | 80, 443, 8080 | 237 |
| 172.67.203.115 | 80, 443, 8080 | 270 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9ae6:76a6:a1a:f53a:ddd:b34e] | 80, 443, 8080 | 4 |
| [2606:4700:8deb:44d1:37b9:7a78:b1c2:496a] | 80, 443, 8080 | 4 |
| [2606:4700:8deb:5ac:1efd:b2ec:c445:7c92] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:50de:8114:c554:5f94:c9bd] | 80, 443, 8080 | 4 |
| [2606:4700:2d:6dbf:d922:8d69:742c:a3ae] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:76a6:a1a:f53a:ddd:b34e] | 80, 443, 8080 | 4 |
| [2606:4700:8deb:44d1:37b9:7a78:b1c2:496a] | 80, 443, 8080 | 4 |
| [2606:4700:8deb:5ac:1efd:b2ec:c445:7c92] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:50de:8114:c554:5f94:c9bd] | 80, 443, 8080 | 4 |
| [2606:4700:2d:6dbf:d922:8d69:742c:a3ae] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:76a6:a1a:f53a:ddd:b34e] | 80, 443, 8080 | 4 |
| [2606:4700:8deb:44d1:37b9:7a78:b1c2:496a] | 80, 443, 8080 | 4 |
| [2606:4700:8deb:5ac:1efd:b2ec:c445:7c92] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:50de:8114:c554:5f94:c9bd] | 80, 443, 8080 | 4 |
| [2606:4700:2d:6dbf:d922:8d69:742c:a3ae] | 80, 443, 8080 | 4 |

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
