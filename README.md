# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-07 13:45:30 +0330

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
| 190.93.247.15 | 80, 443, 8080 | 52 |
| 198.41.208.55 | 80, 443, 8080 | 52 |
| 198.41.208.32 | 80, 443, 8080 | 52 |
| 198.41.215.246 | 80, 443, 8080 | 53 |
| 172.64.94.96 | 80, 443, 8080 | 53 |
| 172.67.65.60 | 80, 443, 8080 | 55 |
| 172.67.88.99 | 80, 443, 8080 | 56 |
| 172.67.76.63 | 80, 443, 8080 | 57 |
| 172.67.138.75 | 80, 443, 8080 | 130 |
| 172.67.223.199 | 80, 443, 8080 | 131 |
| 104.18.223.127 | 80, 443, 8080 | 132 |
| 104.19.60.113 | 80, 443, 8080 | 139 |
| 104.18.216.97 | 80, 443, 8080 | 143 |
| 104.17.55.153 | 80, 443, 8080 | 146 |
| 104.17.158.93 | 80, 443, 8080 | 150 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:839a:9d8:bff8:1ccd:4d65:ae4f] | 80, 443, 8080 | 3 |
| [2606:4700:99ee:fde:a346:48c8:ebcd:d2b6] | 80, 443, 8080 | 3 |
| [2606:4700:839a:9d8:bff8:1ccd:4d65:ae4f] | 80, 443, 8080 | 3 |
| [2606:4700:99ee:fde:a346:48c8:ebcd:d2b6] | 80, 443, 8080 | 3 |
| [2606:4700:839a:9d8:bff8:1ccd:4d65:ae4f] | 80, 443, 8080 | 3 |
| [2606:4700:99ee:fde:a346:48c8:ebcd:d2b6] | 80, 443, 8080 | 3 |
| [2606:4700:9c62:6aa7:9909:d45a:ba28:9ed6] | 80, 443, 8080 | 4 |
| [2606:4700:99ee:3f09:4cbd:5684:a86f:536f] | 80, 443, 8080 | 4 |
| [2606:4700:9c62:d6e8:9c57:fe8f:4b74:659d] | 80, 443, 8080 | 4 |
| [2606:4700:9c62:6aa7:9909:d45a:ba28:9ed6] | 80, 443, 8080 | 4 |
| [2606:4700:99ee:3f09:4cbd:5684:a86f:536f] | 80, 443, 8080 | 4 |
| [2606:4700:9c62:d6e8:9c57:fe8f:4b74:659d] | 80, 443, 8080 | 4 |
| [2606:4700:9c62:6aa7:9909:d45a:ba28:9ed6] | 80, 443, 8080 | 4 |
| [2606:4700:99ee:3f09:4cbd:5684:a86f:536f] | 80, 443, 8080 | 4 |
| [2606:4700:9c62:d6e8:9c57:fe8f:4b74:659d] | 80, 443, 8080 | 4 |

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
