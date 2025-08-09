# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-09 08:43:53 +0330

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
| 172.64.67.9 | 80, 443, 8080 | 52 |
| 162.159.247.9 | 80, 443, 8080 | 53 |
| 162.159.36.43 | 80, 443, 8080 | 54 |
| 162.159.252.210 | 80, 443, 8080 | 54 |
| 162.159.209.130 | 80, 443, 8080 | 64 |
| 172.67.219.183 | 80, 443, 8080 | 130 |
| 172.67.183.168 | 80, 443, 8080 | 131 |
| 172.67.159.128 | 80, 443, 8080 | 131 |
| 172.67.238.107 | 80, 443, 8080 | 131 |
| 104.18.218.167 | 80, 443, 8080 | 133 |
| 104.19.55.38 | 80, 443, 8080 | 137 |
| 104.18.85.51 | 80, 443, 8080 | 139 |
| 104.17.109.47 | 80, 443, 8080 | 142 |
| 104.17.149.50 | 80, 443, 8080 | 145 |
| 172.67.195.29 | 80, 443, 8080 | 220 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9b02:3194:f94:a170:8adf:4db5] | 80, 443, 8080 | 3 |
| [2606:4700:90d9:fabf:c255:17f8:3605:89d5] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:e4c2:3803:413b:7c90:142f] | 80, 443, 8080 | 3 |
| [2606:4700:964e:da5a:3b2f:f9b6:2481:b07a] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:3194:f94:a170:8adf:4db5] | 80, 443, 8080 | 3 |
| [2606:4700:90d9:fabf:c255:17f8:3605:89d5] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:e4c2:3803:413b:7c90:142f] | 80, 443, 8080 | 3 |
| [2606:4700:964e:da5a:3b2f:f9b6:2481:b07a] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:3194:f94:a170:8adf:4db5] | 80, 443, 8080 | 3 |
| [2606:4700:90d9:fabf:c255:17f8:3605:89d5] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:e4c2:3803:413b:7c90:142f] | 80, 443, 8080 | 3 |
| [2606:4700:964e:da5a:3b2f:f9b6:2481:b07a] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:1d4c:ff1c:b120:bd00:10a8] | 80, 443, 8080 | 4 |
| [2606:4700:9a91:1d4c:ff1c:b120:bd00:10a8] | 80, 443, 8080 | 4 |
| [2606:4700:9a91:1d4c:ff1c:b120:bd00:10a8] | 80, 443, 8080 | 4 |

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
