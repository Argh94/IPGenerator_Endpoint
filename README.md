# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-10 18:42:54 +0330

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
| 190.93.246.121 | 80, 443, 8080 | 50 |
| 162.159.255.71 | 80, 443, 8080 | 51 |
| 162.159.241.249 | 80, 443, 8080 | 52 |
| 141.101.115.193 | 80, 443, 8080 | 54 |
| 162.159.192.128 | 80, 443, 8080 | 57 |
| 172.64.89.228 | 80, 443, 8080 | 57 |
| 162.159.129.234 | 80, 443, 8080 | 57 |
| 162.159.251.238 | 80, 443, 8080 | 57 |
| 172.67.156.94 | 80, 443, 8080 | 131 |
| 104.16.66.49 | 80, 443, 8080 | 136 |
| 104.18.97.34 | 80, 443, 8080 | 137 |
| 162.159.244.188 | 80, 443, 8080 | 138 |
| 104.17.70.87 | 80, 443, 8080 | 138 |
| 104.16.159.81 | 80, 443, 8080 | 138 |
| 104.19.95.196 | 80, 443, 8080 | 139 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8dd6:222d:d989:d2d8:1b32:3bcb] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:62ba:94a8:89d1:7ec7:606e] | 80, 443, 8080 | 4 |
| [2606:4700:8dd4:d354:c503:eace:30b2:7349] | 80, 443, 8080 | 4 |
| [2606:4700:91b1:8030:a2b2:127c:a475:4d0c] | 80, 443, 8080 | 4 |
| [2606:4700:8dd6:222d:d989:d2d8:1b32:3bcb] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:62ba:94a8:89d1:7ec7:606e] | 80, 443, 8080 | 4 |
| [2606:4700:8dd4:d354:c503:eace:30b2:7349] | 80, 443, 8080 | 4 |
| [2606:4700:91b1:8030:a2b2:127c:a475:4d0c] | 80, 443, 8080 | 4 |
| [2606:4700:8dd6:222d:d989:d2d8:1b32:3bcb] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:62ba:94a8:89d1:7ec7:606e] | 80, 443, 8080 | 4 |
| [2606:4700:8dd4:d354:c503:eace:30b2:7349] | 80, 443, 8080 | 4 |
| [2606:4700:91b1:8030:a2b2:127c:a475:4d0c] | 80, 443, 8080 | 4 |
| [2606:4700:8dd6:887:ca7e:fb10:e416:c31b] | 80, 443, 8080 | 6 |
| [2606:4700:8dd6:887:ca7e:fb10:e416:c31b] | 80, 443, 8080 | 6 |
| [2606:4700:8dd6:887:ca7e:fb10:e416:c31b] | 80, 443, 8080 | 6 |

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
