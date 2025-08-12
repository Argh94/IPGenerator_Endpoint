# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-12 18:44:46 +0330

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
| 198.41.211.203 | 80, 443, 8080 | 51 |
| 172.64.80.152 | 80, 443, 8080 | 51 |
| 190.93.245.133 | 80, 443, 8080 | 51 |
| 190.93.246.113 | 80, 443, 8080 | 51 |
| 172.67.209.8 | 80, 443, 8080 | 130 |
| 172.67.209.152 | 80, 443, 8080 | 130 |
| 172.64.68.162 | 80, 443, 8080 | 131 |
| 172.67.193.87 | 80, 443, 8080 | 131 |
| 172.67.168.38 | 80, 443, 8080 | 131 |
| 172.67.154.82 | 80, 443, 8080 | 131 |
| 104.19.202.24 | 80, 443, 8080 | 136 |
| 104.17.7.88 | 80, 443, 8080 | 137 |
| 104.19.207.245 | 80, 443, 8080 | 138 |
| 104.19.197.114 | 80, 443, 8080 | 142 |
| 104.18.111.41 | 80, 443, 8080 | 155 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:90cd:3396:aaac:7f61:1f35:e92e] | 80, 443, 8080 | 3 |
| [2606:4700:90cd:3396:aaac:7f61:1f35:e92e] | 80, 443, 8080 | 3 |
| [2606:4700:90cd:3396:aaac:7f61:1f35:e92e] | 80, 443, 8080 | 3 |
| [2606:4700:9a69:4cbc:22a:3d0a:f68d:887d] | 80, 443, 8080 | 4 |
| [2606:4700:9a69:ed6:ceb8:fc56:d5cd:a72d] | 80, 443, 8080 | 4 |
| [2606:4700:9645:82c5:fb25:83b3:9842:88a4] | 80, 443, 8080 | 4 |
| [2606:4700:90cd:9a83:b63f:87f1:0:1800] | 80, 443, 8080 | 4 |
| [2606:4700:9a69:4cbc:22a:3d0a:f68d:887d] | 80, 443, 8080 | 4 |
| [2606:4700:9a69:ed6:ceb8:fc56:d5cd:a72d] | 80, 443, 8080 | 4 |
| [2606:4700:9645:82c5:fb25:83b3:9842:88a4] | 80, 443, 8080 | 4 |
| [2606:4700:90cd:9a83:b63f:87f1:0:1800] | 80, 443, 8080 | 4 |
| [2606:4700:9a69:4cbc:22a:3d0a:f68d:887d] | 80, 443, 8080 | 4 |
| [2606:4700:9a69:ed6:ceb8:fc56:d5cd:a72d] | 80, 443, 8080 | 4 |
| [2606:4700:9645:82c5:fb25:83b3:9842:88a4] | 80, 443, 8080 | 4 |
| [2606:4700:90cd:9a83:b63f:87f1:0:1800] | 80, 443, 8080 | 4 |

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
