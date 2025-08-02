# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-02 08:48:27 +0330

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
| 162.159.136.167 | 80, 443, 8080 | 40 |
| 172.67.118.255 | 80, 443, 8080 | 45 |
| 172.67.79.179 | 80, 443, 8080 | 45 |
| 172.67.178.24 | 80, 443, 8080 | 130 |
| 172.67.202.22 | 80, 443, 8080 | 131 |
| 104.16.69.81 | 80, 443, 8080 | 134 |
| 104.17.49.180 | 80, 443, 8080 | 134 |
| 104.16.69.81 | 80, 443, 8080 | 134 |
| 104.17.49.180 | 80, 443, 8080 | 134 |
| 104.16.133.31 | 80, 443, 8080 | 135 |
| 104.17.193.108 | 80, 443, 8080 | 135 |
| 104.16.133.31 | 80, 443, 8080 | 135 |
| 104.17.193.108 | 80, 443, 8080 | 135 |
| 104.19.255.228 | 80, 443, 8080 | 143 |
| 104.19.255.228 | 80, 443, 8080 | 143 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8d93:c1b:df3b:7d2d:7418:a114] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:cbb7:fc44:f5cb:f824:f92a] | 80, 443, 8080 | 3 |
| [2606:4700:8d93:8adb:71a4:ec3c:caf4:20dc] | 80, 443, 8080 | 3 |
| [2606:4700:8d93:c1b:df3b:7d2d:7418:a114] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:cbb7:fc44:f5cb:f824:f92a] | 80, 443, 8080 | 3 |
| [2606:4700:8d93:8adb:71a4:ec3c:caf4:20dc] | 80, 443, 8080 | 3 |
| [2606:4700:8d93:c1b:df3b:7d2d:7418:a114] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:cbb7:fc44:f5cb:f824:f92a] | 80, 443, 8080 | 3 |
| [2606:4700:8d93:8adb:71a4:ec3c:caf4:20dc] | 80, 443, 8080 | 3 |
| [2606:4700:9a98:d806:dea:d4a7:54cd:1eb8] | 80, 443, 8080 | 4 |
| [2606:4700:54:419d:2d02:4f9e:fb0f:f1a5] | 80, 443, 8080 | 4 |
| [2606:4700:9a98:d806:dea:d4a7:54cd:1eb8] | 80, 443, 8080 | 4 |
| [2606:4700:54:419d:2d02:4f9e:fb0f:f1a5] | 80, 443, 8080 | 4 |
| [2606:4700:9a98:d806:dea:d4a7:54cd:1eb8] | 80, 443, 8080 | 4 |
| [2606:4700:54:419d:2d02:4f9e:fb0f:f1a5] | 80, 443, 8080 | 4 |

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
