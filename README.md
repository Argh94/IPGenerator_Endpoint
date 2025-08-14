# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-14 10:24:29 +0330

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
| 141.101.115.49 | 80, 443, 8080 | 51 |
| 172.64.66.168 | 80, 443, 8080 | 51 |
| 141.101.122.111 | 80, 443, 8080 | 51 |
| 172.64.88.69 | 80, 443, 8080 | 52 |
| 141.101.122.25 | 80, 443, 8080 | 53 |
| 172.64.95.15 | 80, 443, 8080 | 56 |
| 172.67.109.113 | 80, 443, 8080 | 56 |
| 172.67.127.185 | 80, 443, 8080 | 57 |
| 162.159.160.6 | 80, 443, 8080 | 130 |
| 172.67.169.128 | 80, 443, 8080 | 130 |
| 104.19.135.214 | 80, 443, 8080 | 146 |
| 104.24.187.235 | 80, 443, 8080 | 156 |
| 104.27.198.132 | 80, 443, 8080 | 156 |
| 104.18.123.24 | 80, 443, 8080 | 160 |
| 104.19.18.140 | 80, 443, 8080 | 172 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:91b6:efea:4069:d076:7ae9:edd5] | 80, 443, 8080 | 3 |
| [2606:4700:91b6:3fc0:91c8:8041:9d0b:6446] | 80, 443, 8080 | 3 |
| [2606:4700:8d94:44f1:8677:b7bb:aff1:e38a] | 80, 443, 8080 | 3 |
| [2606:4700:91b6:efea:4069:d076:7ae9:edd5] | 80, 443, 8080 | 3 |
| [2606:4700:91b6:3fc0:91c8:8041:9d0b:6446] | 80, 443, 8080 | 3 |
| [2606:4700:8d94:44f1:8677:b7bb:aff1:e38a] | 80, 443, 8080 | 3 |
| [2606:4700:91b6:efea:4069:d076:7ae9:edd5] | 80, 443, 8080 | 3 |
| [2606:4700:91b6:3fc0:91c8:8041:9d0b:6446] | 80, 443, 8080 | 3 |
| [2606:4700:8d94:44f1:8677:b7bb:aff1:e38a] | 80, 443, 8080 | 3 |
| [2606:4700:83b9:5a0b:1932:1bf5:4c82:ab74] | 80, 443, 8080 | 156 |
| [2606:4700:83b9:5a0b:1932:1bf5:4c82:ab74] | 80, 443, 8080 | 156 |
| [2606:4700:83b9:5a0b:1932:1bf5:4c82:ab74] | 80, 443, 8080 | 156 |
| [2606:4700:83b9:24b2:b05a:2e19:8c1d:8ec3] | 80, 443, 8080 | 162 |
| [2606:4700:83b9:24b2:b05a:2e19:8c1d:8ec3] | 80, 443, 8080 | 162 |
| [2606:4700:83b9:24b2:b05a:2e19:8c1d:8ec3] | 80, 443, 8080 | 162 |

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
