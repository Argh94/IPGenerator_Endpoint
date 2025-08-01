# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-01 13:45:30 +0330

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
| 162.159.245.140 | 80, 443, 8080 | 41 |
| 172.64.90.68 | 80, 443, 8080 | 42 |
| 172.67.123.112 | 80, 443, 8080 | 43 |
| 172.67.136.120 | 80, 443, 8080 | 129 |
| 172.67.204.164 | 80, 443, 8080 | 131 |
| 104.19.127.22 | 80, 443, 8080 | 132 |
| 104.19.127.22 | 80, 443, 8080 | 132 |
| 104.17.150.142 | 80, 443, 8080 | 136 |
| 104.17.150.142 | 80, 443, 8080 | 136 |
| 104.19.9.93 | 80, 443, 8080 | 137 |
| 104.19.9.93 | 80, 443, 8080 | 137 |
| 104.17.39.166 | 80, 443, 8080 | 146 |
| 104.17.39.166 | 80, 443, 8080 | 146 |
| 104.18.5.82 | 80, 443, 8080 | 148 |
| 104.18.5.82 | 80, 443, 8080 | 148 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:2a:c5ae:b9b2:72ca:4c68:c029] | 80, 443, 8080 | 3 |
| [2606:4700:8d9c:cc6c:58ef:3b16:31e0:deb8] | 80, 443, 8080 | 3 |
| [2606:4700:9c61:7ec7:986d:d1e2:623e:d377] | 80, 443, 8080 | 3 |
| [2606:4700:2a:c5ae:b9b2:72ca:4c68:c029] | 80, 443, 8080 | 3 |
| [2606:4700:8d9c:cc6c:58ef:3b16:31e0:deb8] | 80, 443, 8080 | 3 |
| [2606:4700:9c61:7ec7:986d:d1e2:623e:d377] | 80, 443, 8080 | 3 |
| [2606:4700:2a:c5ae:b9b2:72ca:4c68:c029] | 80, 443, 8080 | 3 |
| [2606:4700:8d9c:cc6c:58ef:3b16:31e0:deb8] | 80, 443, 8080 | 3 |
| [2606:4700:9c61:7ec7:986d:d1e2:623e:d377] | 80, 443, 8080 | 3 |
| [2606:4700:2a:9425:1c0:56d:9683:6319] | 80, 443, 8080 | 4 |
| [2606:4700:9c61:abd8:69fe:fe82:ddbc:d677] | 80, 443, 8080 | 4 |
| [2606:4700:2a:9425:1c0:56d:9683:6319] | 80, 443, 8080 | 4 |
| [2606:4700:9c61:abd8:69fe:fe82:ddbc:d677] | 80, 443, 8080 | 4 |
| [2606:4700:2a:9425:1c0:56d:9683:6319] | 80, 443, 8080 | 4 |
| [2606:4700:9c61:abd8:69fe:fe82:ddbc:d677] | 80, 443, 8080 | 4 |

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
