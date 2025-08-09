# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-09 13:43:23 +0330

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
| 198.41.209.231 | 80, 443, 8080 | 51 |
| 190.93.247.0 | 80, 443, 8080 | 52 |
| 190.93.244.70 | 80, 443, 8080 | 52 |
| 198.41.209.210 | 80, 443, 8080 | 52 |
| 198.41.209.243 | 80, 443, 8080 | 53 |
| 172.67.119.146 | 80, 443, 8080 | 56 |
| 172.67.86.103 | 80, 443, 8080 | 56 |
| 172.67.65.27 | 80, 443, 8080 | 57 |
| 172.67.105.19 | 80, 443, 8080 | 57 |
| 172.67.197.228 | 80, 443, 8080 | 131 |
| 104.18.207.58 | 80, 443, 8080 | 133 |
| 104.16.231.176 | 80, 443, 8080 | 133 |
| 104.21.234.41 | 80, 443, 8080 | 144 |
| 104.17.96.105 | 80, 443, 8080 | 146 |
| 104.19.20.12 | 80, 443, 8080 | 148 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:13:afce:3827:14bf:ab87:1bef] | 80, 443, 8080 | 3 |
| [2606:4700:9ae7:1a2f:7c52:5c26:42de:be92] | 80, 443, 8080 | 3 |
| [2606:4700:13:afce:3827:14bf:ab87:1bef] | 80, 443, 8080 | 3 |
| [2606:4700:9ae7:1a2f:7c52:5c26:42de:be92] | 80, 443, 8080 | 3 |
| [2606:4700:13:afce:3827:14bf:ab87:1bef] | 80, 443, 8080 | 3 |
| [2606:4700:9ae7:1a2f:7c52:5c26:42de:be92] | 80, 443, 8080 | 3 |
| [2606:4700:13:1981:8f0c:454e:b73b:29eb] | 80, 443, 8080 | 4 |
| [2606:4700:3014:aa37:9eb3:dd62:a16c:4008] | 80, 443, 8080 | 4 |
| [2606:4700:9647:9535:fab0:d5a7:213:d10a] | 80, 443, 8080 | 4 |
| [2606:4700:13:1981:8f0c:454e:b73b:29eb] | 80, 443, 8080 | 4 |
| [2606:4700:3014:aa37:9eb3:dd62:a16c:4008] | 80, 443, 8080 | 4 |
| [2606:4700:9647:9535:fab0:d5a7:213:d10a] | 80, 443, 8080 | 4 |
| [2606:4700:13:1981:8f0c:454e:b73b:29eb] | 80, 443, 8080 | 4 |
| [2606:4700:3014:aa37:9eb3:dd62:a16c:4008] | 80, 443, 8080 | 4 |
| [2606:4700:9647:9535:fab0:d5a7:213:d10a] | 80, 443, 8080 | 4 |

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
