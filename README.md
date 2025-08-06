# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-06 04:40:45 +0330

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
| 172.67.74.195 | 80, 443, 8080 | 57 |
| 141.101.120.168 | 80, 443, 8080 | 131 |
| 141.101.120.168 | 80, 443, 8080 | 131 |
| 172.67.200.232 | 80, 443, 8080 | 131 |
| 172.67.149.211 | 80, 443, 8080 | 131 |
| 172.67.134.238 | 80, 443, 8080 | 131 |
| 172.67.138.61 | 80, 443, 8080 | 131 |
| 104.19.35.214 | 80, 443, 8080 | 134 |
| 104.19.62.107 | 80, 443, 8080 | 134 |
| 104.19.35.214 | 80, 443, 8080 | 134 |
| 104.19.62.107 | 80, 443, 8080 | 134 |
| 104.18.11.17 | 80, 443, 8080 | 139 |
| 104.18.11.17 | 80, 443, 8080 | 139 |
| 104.19.103.37 | 80, 443, 8080 | 141 |
| 104.19.103.37 | 80, 443, 8080 | 141 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8de7:1233:bcc3:25bd:3fce:ae87] | 80, 443, 8080 | 4 |
| [2606:4700:9ada:c17c:ec7b:4815:c230:ad6b] | 80, 443, 8080 | 4 |
| [2606:4700:8de7:39f2:9d45:8994:94d6:2a3e] | 80, 443, 8080 | 4 |
| [2606:4700:9ad0:bf0a:ed97:980e:9b57:f5e4] | 80, 443, 8080 | 4 |
| [2606:4700:3004:cd73:ba49:d0a7:d5fc:ff35] | 80, 443, 8080 | 4 |
| [2606:4700:8de7:1233:bcc3:25bd:3fce:ae87] | 80, 443, 8080 | 4 |
| [2606:4700:9ada:c17c:ec7b:4815:c230:ad6b] | 80, 443, 8080 | 4 |
| [2606:4700:8de7:39f2:9d45:8994:94d6:2a3e] | 80, 443, 8080 | 4 |
| [2606:4700:9ad0:bf0a:ed97:980e:9b57:f5e4] | 80, 443, 8080 | 4 |
| [2606:4700:3004:cd73:ba49:d0a7:d5fc:ff35] | 80, 443, 8080 | 4 |
| [2606:4700:8de7:1233:bcc3:25bd:3fce:ae87] | 80, 443, 8080 | 4 |
| [2606:4700:9ada:c17c:ec7b:4815:c230:ad6b] | 80, 443, 8080 | 4 |
| [2606:4700:8de7:39f2:9d45:8994:94d6:2a3e] | 80, 443, 8080 | 4 |
| [2606:4700:9ad0:bf0a:ed97:980e:9b57:f5e4] | 80, 443, 8080 | 4 |
| [2606:4700:3004:cd73:ba49:d0a7:d5fc:ff35] | 80, 443, 8080 | 4 |

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
