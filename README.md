# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-07-31 08:51:36 +0330

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
| 172.67.70.145 | 80, 443, 8080 | 42 |
| 172.64.91.157 | 80, 443, 8080 | 46 |
| 141.101.114.245 | 80, 443, 8080 | 53 |
| 141.101.121.25 | 80, 443, 8080 | 54 |
| 141.101.115.46 | 80, 443, 8080 | 54 |
| 141.101.114.81 | 80, 443, 8080 | 54 |
| 141.101.115.89 | 80, 443, 8080 | 54 |
| 172.67.238.122 | 80, 443, 8080 | 130 |
| 172.67.170.22 | 80, 443, 8080 | 131 |
| 104.19.36.28 | 80, 443, 8080 | 136 |
| 104.16.219.208 | 80, 443, 8080 | 136 |
| 104.16.202.67 | 80, 443, 8080 | 137 |
| 104.17.241.187 | 80, 443, 8080 | 137 |
| 104.17.240.176 | 80, 443, 8080 | 137 |
| 172.64.96.58 | 80, 443, 8080 | 191 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9ae0:39da:6825:40dd:8a0d:173e] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:40a2:4cda:bdea:a17a:d373] | 80, 443, 8080 | 3 |
| [2606:4700:9ae0:39da:6825:40dd:8a0d:173e] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:40a2:4cda:bdea:a17a:d373] | 80, 443, 8080 | 3 |
| [2606:4700:9ae0:39da:6825:40dd:8a0d:173e] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:40a2:4cda:bdea:a17a:d373] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:ef48:b9b9:5e43:85d1:5f7c] | 80, 443, 8080 | 4 |
| [2606:4700:10:bd30:a1fd:326d:450d:c580] | 80, 443, 8080 | 4 |
| [2606:4700:9ad9:3e2d:6979:1e9d:20bb:db6b] | 80, 443, 8080 | 4 |
| [2606:4700:8dd2:ef48:b9b9:5e43:85d1:5f7c] | 80, 443, 8080 | 4 |
| [2606:4700:10:bd30:a1fd:326d:450d:c580] | 80, 443, 8080 | 4 |
| [2606:4700:9ad9:3e2d:6979:1e9d:20bb:db6b] | 80, 443, 8080 | 4 |
| [2606:4700:8dd2:ef48:b9b9:5e43:85d1:5f7c] | 80, 443, 8080 | 4 |
| [2606:4700:10:bd30:a1fd:326d:450d:c580] | 80, 443, 8080 | 4 |
| [2606:4700:9ad9:3e2d:6979:1e9d:20bb:db6b] | 80, 443, 8080 | 4 |

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
