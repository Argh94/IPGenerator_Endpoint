# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-08 23:45:20 +0330

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
| 172.64.78.212 | 80, 443, 8080 | 56 |
| 162.159.153.106 | 80, 443, 8080 | 58 |
| 190.93.247.206 | 80, 443, 8080 | 59 |
| 104.18.204.33 | 80, 443, 8080 | 128 |
| 104.16.241.28 | 80, 443, 8080 | 128 |
| 104.18.153.254 | 80, 443, 8080 | 131 |
| 172.67.210.220 | 80, 443, 8080 | 131 |
| 172.67.240.122 | 80, 443, 8080 | 131 |
| 104.16.193.58 | 80, 443, 8080 | 133 |
| 104.19.105.246 | 80, 443, 8080 | 138 |
| 162.159.138.0 | 80, 443, 8080 | 202 |
| 172.67.179.130 | 80, 443, 8080 | 203 |
| 172.67.124.117 | 80, 443, 8080 | 206 |
| 172.67.116.248 | 80, 443, 8080 | 206 |
| 172.67.195.205 | 80, 443, 8080 | 217 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8dd9:d657:5849:d9b:caf4:922a] | 80, 443, 8080 | 3 |
| [2606:4700:8d7d:94f8:be96:3e52:87e1:c41b] | 80, 443, 8080 | 3 |
| [2606:4700:8d7d:ea27:3fb0:2113:95e5:2fec] | 80, 443, 8080 | 3 |
| [2606:4700:8dd9:821a:e19:5d22:19aa:626e] | 80, 443, 8080 | 3 |
| [2606:4700:8dd9:d657:5849:d9b:caf4:922a] | 80, 443, 8080 | 3 |
| [2606:4700:8d7d:94f8:be96:3e52:87e1:c41b] | 80, 443, 8080 | 3 |
| [2606:4700:8d7d:ea27:3fb0:2113:95e5:2fec] | 80, 443, 8080 | 3 |
| [2606:4700:8dd9:821a:e19:5d22:19aa:626e] | 80, 443, 8080 | 3 |
| [2606:4700:8dd9:d657:5849:d9b:caf4:922a] | 80, 443, 8080 | 3 |
| [2606:4700:8d7d:94f8:be96:3e52:87e1:c41b] | 80, 443, 8080 | 3 |
| [2606:4700:8d7d:ea27:3fb0:2113:95e5:2fec] | 80, 443, 8080 | 3 |
| [2606:4700:8dd9:821a:e19:5d22:19aa:626e] | 80, 443, 8080 | 3 |
| [2606:4700:90d9:ab28:200e:d4ac:d5e8:566b] | 80, 443, 8080 | 4 |
| [2606:4700:90d9:ab28:200e:d4ac:d5e8:566b] | 80, 443, 8080 | 4 |
| [2606:4700:90d9:ab28:200e:d4ac:d5e8:566b] | 80, 443, 8080 | 4 |

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
