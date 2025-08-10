# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-10 23:44:35 +0330

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
| 172.64.90.232 | 80, 443, 8080 | 51 |
| 162.159.241.249 | 80, 443, 8080 | 52 |
| 190.93.244.194 | 80, 443, 8080 | 52 |
| 141.101.115.193 | 80, 443, 8080 | 54 |
| 172.64.68.122 | 80, 443, 8080 | 55 |
| 172.64.82.108 | 80, 443, 8080 | 57 |
| 104.17.119.157 | 80, 443, 8080 | 130 |
| 172.67.247.101 | 80, 443, 8080 | 131 |
| 172.67.180.230 | 80, 443, 8080 | 131 |
| 172.67.155.38 | 80, 443, 8080 | 131 |
| 104.16.232.110 | 80, 443, 8080 | 132 |
| 104.16.167.145 | 80, 443, 8080 | 132 |
| 104.18.101.226 | 80, 443, 8080 | 132 |
| 172.67.227.140 | 80, 443, 8080 | 132 |
| 104.16.12.92 | 80, 443, 8080 | 134 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9ade:cb36:cc07:a0ed:2104:e9bc] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:bec6:7ca3:6bf9:692f:fe49] | 80, 443, 8080 | 3 |
| [2606:4700:23:a089:b3c2:fcb3:d8fd:8fdb] | 80, 443, 8080 | 3 |
| [2606:4700:23:6f7b:289c:3de2:87a9:4408] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:cb36:cc07:a0ed:2104:e9bc] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:bec6:7ca3:6bf9:692f:fe49] | 80, 443, 8080 | 3 |
| [2606:4700:23:a089:b3c2:fcb3:d8fd:8fdb] | 80, 443, 8080 | 3 |
| [2606:4700:23:6f7b:289c:3de2:87a9:4408] | 80, 443, 8080 | 3 |
| [2606:4700:9ade:cb36:cc07:a0ed:2104:e9bc] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:bec6:7ca3:6bf9:692f:fe49] | 80, 443, 8080 | 3 |
| [2606:4700:23:a089:b3c2:fcb3:d8fd:8fdb] | 80, 443, 8080 | 3 |
| [2606:4700:23:6f7b:289c:3de2:87a9:4408] | 80, 443, 8080 | 3 |
| [2606:4700:99e2:a25b:aeef:72e:5aa8:6547] | 80, 443, 8080 | 4 |
| [2606:4700:99e2:a25b:aeef:72e:5aa8:6547] | 80, 443, 8080 | 4 |
| [2606:4700:99e2:a25b:aeef:72e:5aa8:6547] | 80, 443, 8080 | 4 |

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
