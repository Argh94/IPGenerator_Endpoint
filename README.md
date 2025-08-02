# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-02 13:43:55 +0330

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
| 172.67.68.120 | 80, 443, 8080 | 45 |
| 172.67.78.58 | 80, 443, 8080 | 47 |
| 172.67.233.51 | 80, 443, 8080 | 131 |
| 172.67.241.58 | 80, 443, 8080 | 131 |
| 172.67.223.177 | 80, 443, 8080 | 131 |
| 104.19.20.114 | 80, 443, 8080 | 137 |
| 104.19.191.226 | 80, 443, 8080 | 137 |
| 104.17.118.95 | 80, 443, 8080 | 137 |
| 104.19.20.114 | 80, 443, 8080 | 137 |
| 104.19.191.226 | 80, 443, 8080 | 137 |
| 104.17.118.95 | 80, 443, 8080 | 137 |
| 104.19.78.57 | 80, 443, 8080 | 142 |
| 104.19.78.57 | 80, 443, 8080 | 142 |
| 104.18.21.44 | 80, 443, 8080 | 143 |
| 104.18.21.44 | 80, 443, 8080 | 143 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8d92:fcfb:1516:fe06:9bba:7221] | 80, 443, 8080 | 4 |
| [2606:4700:8d92:34d:de74:447:b46e:c94d] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:b688:7761:fcc0:d7d2:3a57] | 80, 443, 8080 | 4 |
| [2606:4700:3032:c350:8826:940e:4c48:caf4] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:d589:3de8:a336:4301:2e73] | 80, 443, 8080 | 4 |
| [2606:4700:8d92:fcfb:1516:fe06:9bba:7221] | 80, 443, 8080 | 4 |
| [2606:4700:8d92:34d:de74:447:b46e:c94d] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:b688:7761:fcc0:d7d2:3a57] | 80, 443, 8080 | 4 |
| [2606:4700:3032:c350:8826:940e:4c48:caf4] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:d589:3de8:a336:4301:2e73] | 80, 443, 8080 | 4 |
| [2606:4700:8d92:fcfb:1516:fe06:9bba:7221] | 80, 443, 8080 | 4 |
| [2606:4700:8d92:34d:de74:447:b46e:c94d] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:b688:7761:fcc0:d7d2:3a57] | 80, 443, 8080 | 4 |
| [2606:4700:3032:c350:8826:940e:4c48:caf4] | 80, 443, 8080 | 4 |
| [2606:4700:9ae6:d589:3de8:a336:4301:2e73] | 80, 443, 8080 | 4 |

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
