# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-11 08:52:20 +0330

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
| 162.159.251.233 | 80, 443, 8080 | 50 |
| 198.41.208.112 | 80, 443, 8080 | 50 |
| 172.64.90.232 | 80, 443, 8080 | 51 |
| 190.93.244.194 | 80, 443, 8080 | 52 |
| 172.64.68.122 | 80, 443, 8080 | 55 |
| 141.101.113.29 | 80, 443, 8080 | 56 |
| 172.64.81.80 | 80, 443, 8080 | 57 |
| 172.64.67.87 | 80, 443, 8080 | 57 |
| 172.67.231.40 | 80, 443, 8080 | 131 |
| 172.67.158.196 | 80, 443, 8080 | 131 |
| 104.17.227.117 | 80, 443, 8080 | 135 |
| 141.101.123.114 | 80, 443, 8080 | 138 |
| 104.18.217.62 | 80, 443, 8080 | 139 |
| 104.19.248.70 | 80, 443, 8080 | 144 |
| 104.16.112.31 | 80, 443, 8080 | 145 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:4402:fd30:25b3:3544:c240:ea77] | 80, 443, 8080 | 4 |
| [2606:4700:10f:c449:e4ea:73e8:72e4:9584] | 80, 443, 8080 | 4 |
| [2606:4700:9642:b0ab:2a25:9e79:ff4:4bc8] | 80, 443, 8080 | 4 |
| [2606:4700:4402:fd30:25b3:3544:c240:ea77] | 80, 443, 8080 | 4 |
| [2606:4700:10f:c449:e4ea:73e8:72e4:9584] | 80, 443, 8080 | 4 |
| [2606:4700:9642:b0ab:2a25:9e79:ff4:4bc8] | 80, 443, 8080 | 4 |
| [2606:4700:4402:fd30:25b3:3544:c240:ea77] | 80, 443, 8080 | 4 |
| [2606:4700:10f:c449:e4ea:73e8:72e4:9584] | 80, 443, 8080 | 4 |
| [2606:4700:9642:b0ab:2a25:9e79:ff4:4bc8] | 80, 443, 8080 | 4 |
| [2606:4700:3028:d1c5:fb46:36ac:f1d4:36f6] | 80, 443, 8080 | 10 |
| [2606:4700:3028:bbed:1e70:f6f8:3084:64ec] | 80, 443, 8080 | 10 |
| [2606:4700:3028:d1c5:fb46:36ac:f1d4:36f6] | 80, 443, 8080 | 10 |
| [2606:4700:3028:bbed:1e70:f6f8:3084:64ec] | 80, 443, 8080 | 10 |
| [2606:4700:3028:d1c5:fb46:36ac:f1d4:36f6] | 80, 443, 8080 | 10 |
| [2606:4700:3028:bbed:1e70:f6f8:3084:64ec] | 80, 443, 8080 | 10 |

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
