# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-16 00:10:27 +0330

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
| 141.101.121.249 | 80, 443, 8080 | 51 |
| 141.101.122.148 | 80, 443, 8080 | 51 |
| 141.101.120.246 | 80, 443, 8080 | 51 |
| 141.101.114.197 | 80, 443, 8080 | 51 |
| 141.101.114.245 | 80, 443, 8080 | 51 |
| 162.159.193.7 | 80, 443, 8080 | 56 |
| 172.67.110.227 | 80, 443, 8080 | 56 |
| 162.159.232.94 | 80, 443, 8080 | 63 |
| 104.19.165.176 | 80, 443, 8080 | 128 |
| 104.19.43.234 | 80, 443, 8080 | 130 |
| 198.41.223.227 | 80, 443, 8080 | 130 |
| 172.67.213.96 | 80, 443, 8080 | 130 |
| 172.67.212.96 | 80, 443, 8080 | 131 |
| 104.16.174.73 | 80, 443, 8080 | 133 |
| 104.16.0.41 | 80, 443, 8080 | 139 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9640:4b87:18b:6591:8689:2e68] | 80, 443, 8080 | 3 |
| [2606:4700:8dd1:c171:61a:5d3c:afa3:23cf] | 80, 443, 8080 | 3 |
| [2606:4700:9640:59fd:9ab6:7ed4:3015:c03f] | 80, 443, 8080 | 3 |
| [2606:4700:131:6dab:2f73:38b4:c425:a89e] | 80, 443, 8080 | 3 |
| [2606:4700:131:b4f6:74ba:2a89:c592:b3ec] | 80, 443, 8080 | 3 |
| [2606:4700:9640:4b87:18b:6591:8689:2e68] | 80, 443, 8080 | 3 |
| [2606:4700:8dd1:c171:61a:5d3c:afa3:23cf] | 80, 443, 8080 | 3 |
| [2606:4700:9640:59fd:9ab6:7ed4:3015:c03f] | 80, 443, 8080 | 3 |
| [2606:4700:131:6dab:2f73:38b4:c425:a89e] | 80, 443, 8080 | 3 |
| [2606:4700:131:b4f6:74ba:2a89:c592:b3ec] | 80, 443, 8080 | 3 |
| [2606:4700:9640:4b87:18b:6591:8689:2e68] | 80, 443, 8080 | 3 |
| [2606:4700:8dd1:c171:61a:5d3c:afa3:23cf] | 80, 443, 8080 | 3 |
| [2606:4700:9640:59fd:9ab6:7ed4:3015:c03f] | 80, 443, 8080 | 3 |
| [2606:4700:131:6dab:2f73:38b4:c425:a89e] | 80, 443, 8080 | 3 |
| [2606:4700:131:b4f6:74ba:2a89:c592:b3ec] | 80, 443, 8080 | 3 |

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
