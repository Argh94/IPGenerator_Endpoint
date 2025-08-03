# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-03 18:43:24 +0330

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
| 162.159.36.210 | 80, 443, 8080 | 56 |
| 198.41.222.91 | 80, 443, 8080 | 57 |
| 172.67.188.238 | 80, 443, 8080 | 131 |
| 172.67.180.252 | 80, 443, 8080 | 131 |
| 172.67.155.249 | 80, 443, 8080 | 131 |
| 104.19.165.79 | 80, 443, 8080 | 137 |
| 104.19.165.79 | 80, 443, 8080 | 137 |
| 104.19.85.245 | 80, 443, 8080 | 139 |
| 104.19.85.245 | 80, 443, 8080 | 139 |
| 104.16.230.141 | 80, 443, 8080 | 142 |
| 104.16.230.141 | 80, 443, 8080 | 142 |
| 104.18.112.40 | 80, 443, 8080 | 149 |
| 104.18.112.40 | 80, 443, 8080 | 149 |
| 104.25.185.52 | 80, 443, 8080 | 153 |
| 104.25.185.52 | 80, 443, 8080 | 153 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8ca8:964c:840d:fd9b:dc9b:9ee6] | 80, 443, 8080 | 3 |
| [2606:4700:90da:2503:8f45:a2e9:7528:e83c] | 80, 443, 8080 | 3 |
| [2606:4700:90db:9d63:e59:18a:8569:b539] | 80, 443, 8080 | 3 |
| [2606:4700:8ca8:964c:840d:fd9b:dc9b:9ee6] | 80, 443, 8080 | 3 |
| [2606:4700:90da:2503:8f45:a2e9:7528:e83c] | 80, 443, 8080 | 3 |
| [2606:4700:90db:9d63:e59:18a:8569:b539] | 80, 443, 8080 | 3 |
| [2606:4700:8ca8:964c:840d:fd9b:dc9b:9ee6] | 80, 443, 8080 | 3 |
| [2606:4700:90da:2503:8f45:a2e9:7528:e83c] | 80, 443, 8080 | 3 |
| [2606:4700:90db:9d63:e59:18a:8569:b539] | 80, 443, 8080 | 3 |
| [2606:4700:18:a9a5:632e:547c:7469:ba98] | 80, 443, 8080 | 4 |
| [2606:4700:18:25c9:90c6:6fa6:f48b:cf24] | 80, 443, 8080 | 4 |
| [2606:4700:18:a9a5:632e:547c:7469:ba98] | 80, 443, 8080 | 4 |
| [2606:4700:18:25c9:90c6:6fa6:f48b:cf24] | 80, 443, 8080 | 4 |
| [2606:4700:18:a9a5:632e:547c:7469:ba98] | 80, 443, 8080 | 4 |
| [2606:4700:18:25c9:90c6:6fa6:f48b:cf24] | 80, 443, 8080 | 4 |

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
