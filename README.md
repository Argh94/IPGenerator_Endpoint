# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-04 09:02:14 +0330

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
| 162.159.243.79 | 80, 443, 8080 | 45 |
| 172.67.238.131 | 80, 443, 8080 | 130 |
| 172.67.129.5 | 80, 443, 8080 | 131 |
| 172.67.209.255 | 80, 443, 8080 | 131 |
| 172.67.250.5 | 80, 443, 8080 | 131 |
| 104.17.158.140 | 80, 443, 8080 | 138 |
| 104.17.158.140 | 80, 443, 8080 | 138 |
| 104.17.91.132 | 80, 443, 8080 | 141 |
| 104.17.91.132 | 80, 443, 8080 | 141 |
| 104.19.74.53 | 80, 443, 8080 | 147 |
| 104.19.74.53 | 80, 443, 8080 | 147 |
| 104.16.67.20 | 80, 443, 8080 | 149 |
| 104.16.67.20 | 80, 443, 8080 | 149 |
| 104.16.12.77 | 80, 443, 8080 | 150 |
| 104.16.12.77 | 80, 443, 8080 | 150 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9ae2:498c:af8b:365a:a2f8:ac28] | 80, 443, 8080 | 3 |
| [2606:4700:8399:f1df:263a:4f0b:b3a8:1686] | 80, 443, 8080 | 3 |
| [2606:4700:9ae2:498c:af8b:365a:a2f8:ac28] | 80, 443, 8080 | 3 |
| [2606:4700:8399:f1df:263a:4f0b:b3a8:1686] | 80, 443, 8080 | 3 |
| [2606:4700:9ae2:498c:af8b:365a:a2f8:ac28] | 80, 443, 8080 | 3 |
| [2606:4700:8399:f1df:263a:4f0b:b3a8:1686] | 80, 443, 8080 | 3 |
| [2606:4700:3014:b542:fbda:47f:d16a:e2ed] | 80, 443, 8080 | 4 |
| [2606:4700:3014:426e:f17a:92bf:fc8a:6726] | 80, 443, 8080 | 4 |
| [2606:4700:3014:b542:fbda:47f:d16a:e2ed] | 80, 443, 8080 | 4 |
| [2606:4700:3014:426e:f17a:92bf:fc8a:6726] | 80, 443, 8080 | 4 |
| [2606:4700:3014:b542:fbda:47f:d16a:e2ed] | 80, 443, 8080 | 4 |
| [2606:4700:3014:426e:f17a:92bf:fc8a:6726] | 80, 443, 8080 | 4 |
| [2606:4700:83b0:cb9f:a9e4:b0e8:bcbf:b670] | 80, 443, 8080 | 157 |
| [2606:4700:83b0:cb9f:a9e4:b0e8:bcbf:b670] | 80, 443, 8080 | 157 |
| [2606:4700:83b0:cb9f:a9e4:b0e8:bcbf:b670] | 80, 443, 8080 | 157 |

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
