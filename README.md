# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-11 23:44:32 +0330

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
| 198.41.209.14 | 80, 443, 8080 | 51 |
| 162.159.255.192 | 80, 443, 8080 | 56 |
| 172.67.70.195 | 80, 443, 8080 | 57 |
| 162.159.192.55 | 80, 443, 8080 | 57 |
| 198.41.208.113 | 80, 443, 8080 | 75 |
| 162.159.129.243 | 80, 443, 8080 | 76 |
| 104.17.21.222 | 80, 443, 8080 | 127 |
| 104.16.23.201 | 80, 443, 8080 | 129 |
| 104.16.76.194 | 80, 443, 8080 | 130 |
| 104.19.178.254 | 80, 443, 8080 | 130 |
| 104.19.39.196 | 80, 443, 8080 | 130 |
| 172.67.210.159 | 80, 443, 8080 | 130 |
| 172.67.193.196 | 80, 443, 8080 | 131 |
| 162.159.138.254 | 80, 443, 8080 | 134 |
| 198.41.209.152 | 80, 443, 8080 | 138 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:440d:2244:88ed:8ff5:bf48:4e1f] | 80, 443, 8080 | 3 |
| [2606:4700:16:364f:246f:115c:c6b:ac45] | 80, 443, 8080 | 3 |
| [2606:4700:4401:f7b4:aab5:7881:34bd:46f8] | 80, 443, 8080 | 3 |
| [2606:4700:440d:2244:88ed:8ff5:bf48:4e1f] | 80, 443, 8080 | 3 |
| [2606:4700:16:364f:246f:115c:c6b:ac45] | 80, 443, 8080 | 3 |
| [2606:4700:4401:f7b4:aab5:7881:34bd:46f8] | 80, 443, 8080 | 3 |
| [2606:4700:440d:2244:88ed:8ff5:bf48:4e1f] | 80, 443, 8080 | 3 |
| [2606:4700:16:364f:246f:115c:c6b:ac45] | 80, 443, 8080 | 3 |
| [2606:4700:4401:f7b4:aab5:7881:34bd:46f8] | 80, 443, 8080 | 3 |
| [2606:4700:9ad1:f145:a00:d487:80df:13] | 80, 443, 8080 | 4 |
| [2606:4700:9ad1:f145:a00:d487:80df:13] | 80, 443, 8080 | 4 |
| [2606:4700:9ad1:f145:a00:d487:80df:13] | 80, 443, 8080 | 4 |
| [2606:4700:101:94e:763f:f571:d06:e1ec] | 80, 443, 8080 | 9 |
| [2606:4700:101:94e:763f:f571:d06:e1ec] | 80, 443, 8080 | 9 |
| [2606:4700:101:94e:763f:f571:d06:e1ec] | 80, 443, 8080 | 9 |

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
