# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-10 13:43:45 +0330

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
| 190.93.246.198 | 80, 443, 8080 | 51 |
| 172.67.98.148 | 80, 443, 8080 | 56 |
| 172.67.65.210 | 80, 443, 8080 | 56 |
| 162.159.241.52 | 80, 443, 8080 | 57 |
| 162.159.136.185 | 80, 443, 8080 | 77 |
| 162.159.134.173 | 80, 443, 8080 | 88 |
| 190.93.247.130 | 80, 443, 8080 | 99 |
| 172.67.179.90 | 80, 443, 8080 | 130 |
| 172.67.175.60 | 80, 443, 8080 | 131 |
| 104.16.137.77 | 80, 443, 8080 | 134 |
| 104.19.16.206 | 80, 443, 8080 | 135 |
| 104.16.65.78 | 80, 443, 8080 | 135 |
| 104.19.202.69 | 80, 443, 8080 | 136 |
| 104.16.11.201 | 80, 443, 8080 | 137 |
| 162.159.244.188 | 80, 443, 8080 | 138 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9ae6:ccc2:473:367e:ef96:a0f] | 80, 443, 8080 | 3 |
| [2606:4700:9a9b:b9a0:6d20:301c:7999:1e78] | 80, 443, 8080 | 3 |
| [2606:4700:91ba:4006:9fb4:d87a:20f6:cff7] | 80, 443, 8080 | 3 |
| [2606:4700:9a9b:acf6:b8e2:c673:6672:358f] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:ccc2:473:367e:ef96:a0f] | 80, 443, 8080 | 3 |
| [2606:4700:9a9b:b9a0:6d20:301c:7999:1e78] | 80, 443, 8080 | 3 |
| [2606:4700:91ba:4006:9fb4:d87a:20f6:cff7] | 80, 443, 8080 | 3 |
| [2606:4700:9a9b:acf6:b8e2:c673:6672:358f] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:ccc2:473:367e:ef96:a0f] | 80, 443, 8080 | 3 |
| [2606:4700:9a9b:b9a0:6d20:301c:7999:1e78] | 80, 443, 8080 | 3 |
| [2606:4700:91ba:4006:9fb4:d87a:20f6:cff7] | 80, 443, 8080 | 3 |
| [2606:4700:9a9b:acf6:b8e2:c673:6672:358f] | 80, 443, 8080 | 3 |
| [2606:4700:91ba:3a9e:beaa:74b1:daf7:25e3] | 80, 443, 8080 | 4 |
| [2606:4700:91ba:3a9e:beaa:74b1:daf7:25e3] | 80, 443, 8080 | 4 |
| [2606:4700:91ba:3a9e:beaa:74b1:daf7:25e3] | 80, 443, 8080 | 4 |

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
