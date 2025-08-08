# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-08 04:41:06 +0330

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
| 190.93.247.15 | 80, 443, 8080 | 52 |
| 198.41.208.55 | 80, 443, 8080 | 52 |
| 198.41.208.32 | 80, 443, 8080 | 52 |
| 198.41.215.246 | 80, 443, 8080 | 53 |
| 172.64.94.96 | 80, 443, 8080 | 53 |
| 172.67.103.89 | 80, 443, 8080 | 56 |
| 141.101.115.36 | 80, 443, 8080 | 57 |
| 162.159.129.92 | 80, 443, 8080 | 57 |
| 104.18.195.139 | 80, 443, 8080 | 130 |
| 104.16.6.202 | 80, 443, 8080 | 131 |
| 172.67.135.203 | 80, 443, 8080 | 131 |
| 172.67.230.197 | 80, 443, 8080 | 131 |
| 104.17.206.86 | 80, 443, 8080 | 132 |
| 104.16.14.254 | 80, 443, 8080 | 133 |
| 104.19.151.232 | 80, 443, 8080 | 135 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8391:3b50:6b0c:901d:30ec:d30c] | 80, 443, 8080 | 3 |
| [2606:4700:9a90:d2b5:d43d:3f8c:6c93:aa10] | 80, 443, 8080 | 3 |
| [2606:4700:8ca0:83b9:4a4d:3594:7213:3501] | 80, 443, 8080 | 3 |
| [2606:4700:8391:3b50:6b0c:901d:30ec:d30c] | 80, 443, 8080 | 3 |
| [2606:4700:9a90:d2b5:d43d:3f8c:6c93:aa10] | 80, 443, 8080 | 3 |
| [2606:4700:8ca0:83b9:4a4d:3594:7213:3501] | 80, 443, 8080 | 3 |
| [2606:4700:8391:3b50:6b0c:901d:30ec:d30c] | 80, 443, 8080 | 3 |
| [2606:4700:9a90:d2b5:d43d:3f8c:6c93:aa10] | 80, 443, 8080 | 3 |
| [2606:4700:8ca0:83b9:4a4d:3594:7213:3501] | 80, 443, 8080 | 3 |
| [2606:4700:9a90:3678:1ddb:2f22:fdb7:7d9f] | 80, 443, 8080 | 4 |
| [2606:4700:8d7c:51e:8932:3d18:f5ce:1c27] | 80, 443, 8080 | 4 |
| [2606:4700:9a90:3678:1ddb:2f22:fdb7:7d9f] | 80, 443, 8080 | 4 |
| [2606:4700:8d7c:51e:8932:3d18:f5ce:1c27] | 80, 443, 8080 | 4 |
| [2606:4700:9a90:3678:1ddb:2f22:fdb7:7d9f] | 80, 443, 8080 | 4 |
| [2606:4700:8d7c:51e:8932:3d18:f5ce:1c27] | 80, 443, 8080 | 4 |

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
