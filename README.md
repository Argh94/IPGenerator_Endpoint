# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0%2B-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN یا بهبود عملکرد شبکه مناسب هستند.

**آخرین به‌روزرسانی:** 2025-08-16 00:47:25 +0330

**فایل‌های JSON**: فایل‌های `ipv4.json`، `ipv6.json` و `export.json` در پوشه `list` یا [بخش Releases](https://github.com/Argh94/IPOptimizer/releases) در دسترس هستند.

## ✨ ویژگی‌ها
- 📡 **IPهای کم‌تأخیر**: مرتب‌سازی IPها بر اساس کمترین latency.
- 🔍 **بررسی پورت‌ها**: پورت‌های باز (80، 443، 8080) به‌صورت خودکار بررسی می‌شوند.
- ⏰ **به‌روزرسانی منظم**: به‌روزرسانی خودکار هر ۵ ساعت با GitHub Actions.
- 📄 **خروجی JSON**: ذخیره‌سازی داده‌ها در فایل‌های `ipv4.json`، `ipv6.json` و `export.json`.

## 📋 IPهای بهینه

**توجه:** پورت‌های نمایش‌داده‌شده توسط اسکریپت بررسی شده‌اند، اما بسته به شبکه شما ممکن است متفاوت باشند. برای تأیید، از ابزارهایی مانند [YouGetSignal](https://www.yougetsignal.com/tools/open-ports/) برای IPv4 یا [Nmap](https://nmap.org/) برای IPv6 استفاده کنید.

<div align="center">

### IPv4
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| 141.101.121.249 | 80, 443, 8080 | 51 |
| 141.101.122.148 | 80, 443, 8080 | 51 |
| 141.101.120.246 | 80, 443, 8080 | 51 |
| 141.101.114.197 | 80, 443, 8080 | 51 |
| 141.101.114.245 | 80, 443, 8080 | 51 |
| 162.159.36.245 | 80, 443, 8080 | 56 |
| 172.67.66.4 | 80, 443, 8080 | 56 |
| 190.93.244.23 | 80, 443, 8080 | 57 |
| 104.18.167.106 | 80, 443, 8080 | 129 |
| 104.17.196.243 | 80, 443, 8080 | 129 |
| 172.67.188.197 | 80, 443, 8080 | 130 |
| 172.67.213.96 | 80, 443, 8080 | 130 |
| 104.19.202.24 | 80, 443, 8080 | 132 |
| 104.17.37.205 | 80, 443, 8080 | 135 |
| 104.16.0.41 | 80, 443, 8080 | 139 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:1c:216:abfc:e15b:422c:6530] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:ccc2:a4c5:e2a6:7ec8:6c75] | 80, 443, 8080 | 3 |
| [2606:4700:1c:93fd:9fa5:d8dc:d3f9:a204] | 80, 443, 8080 | 3 |
| [2606:4700:9647:a8a6:cebb:cf75:6cda:303e] | 80, 443, 8080 | 3 |
| [2606:4700:9647:b367:eb3f:37b1:fe66:cce5] | 80, 443, 8080 | 3 |
| [2606:4700:1c:216:abfc:e15b:422c:6530] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:ccc2:a4c5:e2a6:7ec8:6c75] | 80, 443, 8080 | 3 |
| [2606:4700:1c:93fd:9fa5:d8dc:d3f9:a204] | 80, 443, 8080 | 3 |
| [2606:4700:9647:a8a6:cebb:cf75:6cda:303e] | 80, 443, 8080 | 3 |
| [2606:4700:9647:b367:eb3f:37b1:fe66:cce5] | 80, 443, 8080 | 3 |
| [2606:4700:1c:216:abfc:e15b:422c:6530] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:ccc2:a4c5:e2a6:7ec8:6c75] | 80, 443, 8080 | 3 |
| [2606:4700:1c:93fd:9fa5:d8dc:d3f9:a204] | 80, 443, 8080 | 3 |
| [2606:4700:9647:a8a6:cebb:cf75:6cda:303e] | 80, 443, 8080 | 3 |
| [2606:4700:9647:b367:eb3f:37b1:fe66:cce5] | 80, 443, 8080 | 3 |

</div>
## 🛠️ نصب و استفاده
1. **کلون کردن مخزن**:
   ```bash
   git clone https://github.com/Argh94/IPOptimizer.git
   cd IPOptimizer
   ```
2. **تنظیمات PHP**:
   - PHP 8.0 یا بالاتر نصب کنید.
   - کلید API Hostmonit را در متغیر محیطی `HOSTMONIT_API_KEY` تنظیم کنید:
     ```bash
     export HOSTMONIT_API_KEY="your-api-key"
     ```
   - (اختیاری) مسیر ذخیره‌سازی فایل‌های JSON را با متغیر محیطی `LIST_DIR` تنظیم کنید:
     ```bash
     export LIST_DIR="your-custom-path"
     ```
3. **اجرای اسکریپت**:
   ```bash
   php scripts/fetch_ips.php
   ```
4. **بررسی خروجی**:
   - فایل‌های JSON (`ipv4.json`، `ipv6.json`، `export.json`) در پوشه `list` یا [بخش Releases](https://github.com/Argh94/IPOptimizer/releases) در دسترس هستند.
   - لیست IPها در `README.md` به‌روزرسانی می‌شود.

## 📬 پشتیبانی
- 🐛 **گزارش مشکلات**: [Issues](https://github.com/Argh94/IPOptimizer/issues)
- 📧 **تماس**: [ircfspace@gmail.com](mailto:ircfspace@gmail.com)

## 📄 لایسنس
این پروژه تحت [لایسنس MIT](https://opensource.org/licenses/MIT) منتشر شده است.
