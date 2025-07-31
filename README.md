# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-07-31 18:45:21 +0330

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
| 172.67.127.115 | 80, 443, 8080 | 39 |
| 172.67.127.93 | 80, 443, 8080 | 41 |
| 172.64.81.231 | 80, 443, 8080 | 46 |
| 141.101.114.245 | 80, 443, 8080 | 53 |
| 141.101.121.25 | 80, 443, 8080 | 54 |
| 141.101.115.46 | 80, 443, 8080 | 54 |
| 141.101.115.89 | 80, 443, 8080 | 54 |
| 141.101.114.81 | 80, 443, 8080 | 54 |
| 172.67.151.78 | 80, 443, 8080 | 130 |
| 172.67.141.228 | 80, 443, 8080 | 131 |
| 104.17.112.26 | 80, 443, 8080 | 137 |
| 104.17.109.10 | 80, 443, 8080 | 138 |
| 104.16.139.208 | 80, 443, 8080 | 146 |
| 104.18.122.25 | 80, 443, 8080 | 151 |
| 104.19.45.65 | 80, 443, 8080 | 155 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:d:ea95:58e1:79fc:5d1c:221] | 80, 443, 8080 | 3 |
| [2606:4700:d:ea95:58e1:79fc:5d1c:221] | 80, 443, 8080 | 3 |
| [2606:4700:d:ea95:58e1:79fc:5d1c:221] | 80, 443, 8080 | 3 |
| [2606:4700:9ad6:bdd9:8823:471b:f53e:6bbc] | 80, 443, 8080 | 4 |
| [2606:4700:2d:2063:adbe:f452:acf8:9c35] | 80, 443, 8080 | 4 |
| [2606:4700:9a9a:bf54:4bd4:5700:30b7:ea72] | 80, 443, 8080 | 4 |
| [2606:4700:9ad6:4553:8108:dfd6:3fc7:97b] | 80, 443, 8080 | 4 |
| [2606:4700:9ad6:bdd9:8823:471b:f53e:6bbc] | 80, 443, 8080 | 4 |
| [2606:4700:2d:2063:adbe:f452:acf8:9c35] | 80, 443, 8080 | 4 |
| [2606:4700:9a9a:bf54:4bd4:5700:30b7:ea72] | 80, 443, 8080 | 4 |
| [2606:4700:9ad6:4553:8108:dfd6:3fc7:97b] | 80, 443, 8080 | 4 |
| [2606:4700:9ad6:bdd9:8823:471b:f53e:6bbc] | 80, 443, 8080 | 4 |
| [2606:4700:2d:2063:adbe:f452:acf8:9c35] | 80, 443, 8080 | 4 |
| [2606:4700:9a9a:bf54:4bd4:5700:30b7:ea72] | 80, 443, 8080 | 4 |
| [2606:4700:9ad6:4553:8108:dfd6:3fc7:97b] | 80, 443, 8080 | 4 |

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
