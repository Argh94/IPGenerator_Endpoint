# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-05 08:53:48 +0330

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
| 172.67.115.46 | 80, 443, 8080 | 56 |
| 172.67.76.182 | 80, 443, 8080 | 56 |
| 172.64.91.85 | 80, 443, 8080 | 57 |
| 172.67.111.151 | 80, 443, 8080 | 57 |
| 172.67.139.209 | 80, 443, 8080 | 130 |
| 104.21.104.148 | 80, 443, 8080 | 153 |
| 104.21.104.148 | 80, 443, 8080 | 153 |
| 104.18.17.251 | 80, 443, 8080 | 156 |
| 104.18.17.251 | 80, 443, 8080 | 156 |
| 162.159.247.190 | 80, 443, 8080 | 159 |
| 162.159.247.190 | 80, 443, 8080 | 159 |
| 104.21.45.106 | 80, 443, 8080 | 162 |
| 104.21.45.106 | 80, 443, 8080 | 162 |
| 172.67.153.112 | 80, 443, 8080 | 164 |
| 172.67.153.112 | 80, 443, 8080 | 164 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:90cc:9abf:b3d8:419b:8694:2504] | 80, 443, 8080 | 3 |
| [2606:4700:8cac:9658:d214:16fc:d050:5a27] | 80, 443, 8080 | 3 |
| [2606:4700:8de4:879d:46a6:ffb3:6d19:4a13] | 80, 443, 8080 | 3 |
| [2606:4700:8cac:14c1:8589:75c6:1907:74bd] | 80, 443, 8080 | 3 |
| [2606:4700:90cc:9abf:b3d8:419b:8694:2504] | 80, 443, 8080 | 3 |
| [2606:4700:8cac:9658:d214:16fc:d050:5a27] | 80, 443, 8080 | 3 |
| [2606:4700:8de4:879d:46a6:ffb3:6d19:4a13] | 80, 443, 8080 | 3 |
| [2606:4700:8cac:14c1:8589:75c6:1907:74bd] | 80, 443, 8080 | 3 |
| [2606:4700:90cc:9abf:b3d8:419b:8694:2504] | 80, 443, 8080 | 3 |
| [2606:4700:8cac:9658:d214:16fc:d050:5a27] | 80, 443, 8080 | 3 |
| [2606:4700:8de4:879d:46a6:ffb3:6d19:4a13] | 80, 443, 8080 | 3 |
| [2606:4700:8cac:14c1:8589:75c6:1907:74bd] | 80, 443, 8080 | 3 |
| [2606:4700:8de4:bba1:b45:8ac2:b90e:8a43] | 80, 443, 8080 | 4 |
| [2606:4700:8de4:bba1:b45:8ac2:b90e:8a43] | 80, 443, 8080 | 4 |
| [2606:4700:8de4:bba1:b45:8ac2:b90e:8a43] | 80, 443, 8080 | 4 |

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
