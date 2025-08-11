# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-11 18:45:38 +0330

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
| 162.159.246.165 | 80, 443, 8080 | 51 |
| 141.101.114.218 | 80, 443, 8080 | 55 |
| 190.93.245.158 | 80, 443, 8080 | 55 |
| 141.101.114.170 | 80, 443, 8080 | 55 |
| 162.159.240.111 | 80, 443, 8080 | 56 |
| 162.159.248.6 | 80, 443, 8080 | 56 |
| 172.67.112.171 | 80, 443, 8080 | 56 |
| 162.159.134.76 | 80, 443, 8080 | 76 |
| 172.67.148.188 | 80, 443, 8080 | 131 |
| 172.67.255.62 | 80, 443, 8080 | 131 |
| 104.19.149.29 | 80, 443, 8080 | 134 |
| 104.16.8.227 | 80, 443, 8080 | 134 |
| 104.19.169.124 | 80, 443, 8080 | 137 |
| 104.17.79.49 | 80, 443, 8080 | 139 |
| 104.17.235.79 | 80, 443, 8080 | 141 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8d74:4dcd:5561:aec6:be21:7dd2] | 80, 443, 8080 | 3 |
| [2606:4700:440c:7b4f:1fa9:a1ba:ab91:dd10] | 80, 443, 8080 | 3 |
| [2606:4700:8d74:4dcd:5561:aec6:be21:7dd2] | 80, 443, 8080 | 3 |
| [2606:4700:440c:7b4f:1fa9:a1ba:ab91:dd10] | 80, 443, 8080 | 3 |
| [2606:4700:8d74:4dcd:5561:aec6:be21:7dd2] | 80, 443, 8080 | 3 |
| [2606:4700:440c:7b4f:1fa9:a1ba:ab91:dd10] | 80, 443, 8080 | 3 |
| [2606:4700:10f:503e:540f:1cb3:30dc:330e] | 80, 443, 8080 | 4 |
| [2606:4700:440a:bfed:fa14:87f:1f7f:4e61] | 80, 443, 8080 | 4 |
| [2606:4700:10f:e2b:2415:d959:791f:468] | 80, 443, 8080 | 4 |
| [2606:4700:10f:503e:540f:1cb3:30dc:330e] | 80, 443, 8080 | 4 |
| [2606:4700:440a:bfed:fa14:87f:1f7f:4e61] | 80, 443, 8080 | 4 |
| [2606:4700:10f:e2b:2415:d959:791f:468] | 80, 443, 8080 | 4 |
| [2606:4700:10f:503e:540f:1cb3:30dc:330e] | 80, 443, 8080 | 4 |
| [2606:4700:440a:bfed:fa14:87f:1f7f:4e61] | 80, 443, 8080 | 4 |
| [2606:4700:10f:e2b:2415:d959:791f:468] | 80, 443, 8080 | 4 |

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
