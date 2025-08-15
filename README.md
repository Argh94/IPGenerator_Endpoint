# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-15 10:23:49 +0330

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
| 141.101.121.249 | 80, 443, 8080 | 51 |
| 141.101.122.148 | 80, 443, 8080 | 51 |
| 141.101.120.246 | 80, 443, 8080 | 51 |
| 141.101.114.197 | 80, 443, 8080 | 51 |
| 141.101.114.245 | 80, 443, 8080 | 51 |
| 172.64.84.96 | 80, 443, 8080 | 56 |
| 172.67.95.120 | 80, 443, 8080 | 56 |
| 172.64.67.44 | 80, 443, 8080 | 57 |
| 172.67.173.26 | 80, 443, 8080 | 130 |
| 172.67.147.66 | 80, 443, 8080 | 131 |
| 104.21.235.5 | 80, 443, 8080 | 146 |
| 104.19.28.76 | 80, 443, 8080 | 161 |
| 173.245.49.12 | 80, 443, 8080 | 161 |
| 104.18.122.99 | 80, 443, 8080 | 164 |
| 104.25.107.127 | 80, 443, 8080 | 174 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9643:d3d2:62b8:94ec:c837:7e5b] | 80, 443, 8080 | 4 |
| [2606:4700:90c0:af20:bc37:925b:d47a:728a] | 80, 443, 8080 | 4 |
| [2606:4700:90c3:59ac:eefa:4be9:5326:ebbd] | 80, 443, 8080 | 4 |
| [2606:4700:9643:d3d2:62b8:94ec:c837:7e5b] | 80, 443, 8080 | 4 |
| [2606:4700:90c0:af20:bc37:925b:d47a:728a] | 80, 443, 8080 | 4 |
| [2606:4700:90c3:59ac:eefa:4be9:5326:ebbd] | 80, 443, 8080 | 4 |
| [2606:4700:9643:d3d2:62b8:94ec:c837:7e5b] | 80, 443, 8080 | 4 |
| [2606:4700:90c0:af20:bc37:925b:d47a:728a] | 80, 443, 8080 | 4 |
| [2606:4700:90c3:59ac:eefa:4be9:5326:ebbd] | 80, 443, 8080 | 4 |
| [2606:4700:83bb:6a87:f669:f901:3f44:b471] | 80, 443, 8080 | 154 |
| [2606:4700:83bb:6a87:f669:f901:3f44:b471] | 80, 443, 8080 | 154 |
| [2606:4700:83bb:6a87:f669:f901:3f44:b471] | 80, 443, 8080 | 154 |
| [2606:4700:83bb:b367:7303:bfe1:d58e:ea18] | 80, 443, 8080 | 156 |
| [2606:4700:83bb:b367:7303:bfe1:d58e:ea18] | 80, 443, 8080 | 156 |
| [2606:4700:83bb:b367:7303:bfe1:d58e:ea18] | 80, 443, 8080 | 156 |

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
