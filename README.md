# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-07-31 04:40:33 +0330

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
| 172.67.74.64 | 80, 443, 8080 | 40 |
| 172.64.81.125 | 80, 443, 8080 | 44 |
| 141.101.114.245 | 80, 443, 8080 | 53 |
| 141.101.121.25 | 80, 443, 8080 | 54 |
| 141.101.115.46 | 80, 443, 8080 | 54 |
| 141.101.115.89 | 80, 443, 8080 | 54 |
| 141.101.114.81 | 80, 443, 8080 | 54 |
| 104.16.0.10 | 80, 443, 8080 | 130 |
| 172.67.231.85 | 80, 443, 8080 | 130 |
| 172.67.198.129 | 80, 443, 8080 | 131 |
| 172.67.148.160 | 80, 443, 8080 | 131 |
| 104.17.65.87 | 80, 443, 8080 | 132 |
| 104.18.228.31 | 80, 443, 8080 | 132 |
| 104.17.69.208 | 80, 443, 8080 | 132 |
| 104.19.88.254 | 80, 443, 8080 | 133 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:90d1:13d2:510a:5a4d:eb1a:9cf1] | 80, 443, 8080 | 3 |
| [2606:4700:13:5d1a:ea7d:19f1:e761:928] | 80, 443, 8080 | 3 |
| [2606:4700:8391:ce32:735f:cadb:e306:c4fa] | 80, 443, 8080 | 3 |
| [2606:4700:90d1:13d2:510a:5a4d:eb1a:9cf1] | 80, 443, 8080 | 3 |
| [2606:4700:13:5d1a:ea7d:19f1:e761:928] | 80, 443, 8080 | 3 |
| [2606:4700:8391:ce32:735f:cadb:e306:c4fa] | 80, 443, 8080 | 3 |
| [2606:4700:90d1:13d2:510a:5a4d:eb1a:9cf1] | 80, 443, 8080 | 3 |
| [2606:4700:13:5d1a:ea7d:19f1:e761:928] | 80, 443, 8080 | 3 |
| [2606:4700:8391:ce32:735f:cadb:e306:c4fa] | 80, 443, 8080 | 3 |
| [2606:4700:9ad5:b245:15d4:9000:15:3b55] | 80, 443, 8080 | 4 |
| [2606:4700:13:d658:8f92:2cfd:55f2:bd3c] | 80, 443, 8080 | 4 |
| [2606:4700:9ad5:b245:15d4:9000:15:3b55] | 80, 443, 8080 | 4 |
| [2606:4700:13:d658:8f92:2cfd:55f2:bd3c] | 80, 443, 8080 | 4 |
| [2606:4700:9ad5:b245:15d4:9000:15:3b55] | 80, 443, 8080 | 4 |
| [2606:4700:13:d658:8f92:2cfd:55f2:bd3c] | 80, 443, 8080 | 4 |

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
