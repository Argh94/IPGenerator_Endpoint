# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-09 23:44:05 +0330

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
| 162.159.241.246 | 80, 443, 8080 | 50 |
| 172.64.93.156 | 80, 443, 8080 | 53 |
| 172.64.95.130 | 80, 443, 8080 | 54 |
| 162.159.252.192 | 80, 443, 8080 | 54 |
| 162.159.134.175 | 80, 443, 8080 | 55 |
| 172.67.68.108 | 80, 443, 8080 | 56 |
| 162.159.247.75 | 80, 443, 8080 | 57 |
| 162.159.254.188 | 80, 443, 8080 | 57 |
| 198.41.208.148 | 80, 443, 8080 | 100 |
| 104.17.166.76 | 80, 443, 8080 | 128 |
| 104.19.189.106 | 80, 443, 8080 | 129 |
| 104.16.99.127 | 80, 443, 8080 | 130 |
| 172.67.227.234 | 80, 443, 8080 | 131 |
| 104.17.208.213 | 80, 443, 8080 | 133 |
| 104.18.175.247 | 80, 443, 8080 | 133 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:91b9:5934:e725:b77a:1039:621f] | 80, 443, 8080 | 3 |
| [2606:4700:91b9:e298:e1c8:6395:5bdb:2a11] | 80, 443, 8080 | 3 |
| [2606:4700:101:7afd:953d:a6d8:c8c2:bca6] | 80, 443, 8080 | 3 |
| [2606:4700:4407:c9e4:b7f5:fe6:7362:2313] | 80, 443, 8080 | 3 |
| [2606:4700:91b9:5934:e725:b77a:1039:621f] | 80, 443, 8080 | 3 |
| [2606:4700:91b9:e298:e1c8:6395:5bdb:2a11] | 80, 443, 8080 | 3 |
| [2606:4700:101:7afd:953d:a6d8:c8c2:bca6] | 80, 443, 8080 | 3 |
| [2606:4700:4407:c9e4:b7f5:fe6:7362:2313] | 80, 443, 8080 | 3 |
| [2606:4700:91b9:5934:e725:b77a:1039:621f] | 80, 443, 8080 | 3 |
| [2606:4700:91b9:e298:e1c8:6395:5bdb:2a11] | 80, 443, 8080 | 3 |
| [2606:4700:101:7afd:953d:a6d8:c8c2:bca6] | 80, 443, 8080 | 3 |
| [2606:4700:4407:c9e4:b7f5:fe6:7362:2313] | 80, 443, 8080 | 3 |
| [2606:4700:9b08:a58f:955b:f756:b2bf:da45] | 80, 443, 8080 | 4 |
| [2606:4700:9b08:a58f:955b:f756:b2bf:da45] | 80, 443, 8080 | 4 |
| [2606:4700:9b08:a58f:955b:f756:b2bf:da45] | 80, 443, 8080 | 4 |

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
