# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-16 01:25:31 +0330

**فایل‌های JSON**: فایل‌های `ipv4.json`، `ipv6.json` و `export.json` در [بخش Releases](https://github.com/Argh94/IPOptimizer/releases) در دسترس هستند.

## ✨ ویژگی‌ها
- 📡 **IPهای کم‌تأخیر**: مرتب‌شده بر اساس کمترین latency.
- 🔍 **پورت‌های پیشنهادی**: پورت‌های باز (80، 443، 8080) به‌صورت خودکار بررسی می‌شوند.
- ⏰ **به‌روزرسانی منظم**: هر ۵ ساعت با GitHub Actions.
- 📄 **خروجی‌های JSON**: داده‌ها در بخش Releases (`ipv4.json`، `ipv6.json`، `export.json`) ذخیره می‌شوند.

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
| 172.64.83.233 | 80, 443, 8080 | 56 |
| 172.67.66.4 | 80, 443, 8080 | 56 |
| 190.93.244.23 | 80, 443, 8080 | 57 |
| 190.93.246.127 | 80, 443, 8080 | 57 |
| 104.18.66.1 | 80, 443, 8080 | 128 |
| 104.18.167.106 | 80, 443, 8080 | 129 |
| 104.17.196.243 | 80, 443, 8080 | 129 |
| 104.17.34.19 | 80, 443, 8080 | 130 |
| 172.67.224.176 | 80, 443, 8080 | 131 |
| 104.19.59.40 | 80, 443, 8080 | 132 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8dd2:892a:4725:ad83:ce33:bb34] | 80, 443, 8080 | 3 |
| [2606:4700:2e:21ee:1810:d7b7:cf3d:2d3d] | 80, 443, 8080 | 3 |
| [2606:4700:8d92:aee:2ef7:24de:f030:faf8] | 80, 443, 8080 | 3 |
| [2606:4700:19:c8e3:df67:9055:aff0:81ef] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:892a:4725:ad83:ce33:bb34] | 80, 443, 8080 | 3 |
| [2606:4700:2e:21ee:1810:d7b7:cf3d:2d3d] | 80, 443, 8080 | 3 |
| [2606:4700:8d92:aee:2ef7:24de:f030:faf8] | 80, 443, 8080 | 3 |
| [2606:4700:19:c8e3:df67:9055:aff0:81ef] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:892a:4725:ad83:ce33:bb34] | 80, 443, 8080 | 3 |
| [2606:4700:2e:21ee:1810:d7b7:cf3d:2d3d] | 80, 443, 8080 | 3 |
| [2606:4700:8d92:aee:2ef7:24de:f030:faf8] | 80, 443, 8080 | 3 |
| [2606:4700:19:c8e3:df67:9055:aff0:81ef] | 80, 443, 8080 | 3 |
| [2606:4700:8dd2:3004:8156:93d5:754f:cc66] | 80, 443, 8080 | 5 |
| [2606:4700:8dd2:3004:8156:93d5:754f:cc66] | 80, 443, 8080 | 5 |
| [2606:4700:8dd2:3004:8156:93d5:754f:cc66] | 80, 443, 8080 | 5 |

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
   - فایل‌های JSON در [بخش Releases](https://github.com/Argh94/IPOptimizer/releases) در دسترس هستند.
   - لیست IPها در `README.md`.

## 📬 پشتیبانی
- 🐛 **گزارش مشکلات**: [Issues](https://github.com/Argh94/IPOptimizer/issues)
- 📧 **تماس**: [ircfspace@gmail.com](mailto:ircfspace@gmail.com)

## 📄 لایسنس
این پروژه تحت [لایسنس MIT](https://github.com/Argh94/HandWave/blob/main/LICENCE) منتشر شده است.
