# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-07 23:45:33 +0330

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
| 198.41.208.32 | 80, 443, 8080 | 52 |
| 198.41.208.55 | 80, 443, 8080 | 52 |
| 198.41.215.246 | 80, 443, 8080 | 53 |
| 172.64.94.96 | 80, 443, 8080 | 53 |
| 172.64.89.100 | 80, 443, 8080 | 56 |
| 172.67.106.237 | 80, 443, 8080 | 56 |
| 172.67.118.17 | 80, 443, 8080 | 57 |
| 104.19.60.6 | 80, 443, 8080 | 129 |
| 104.18.210.52 | 80, 443, 8080 | 130 |
| 104.19.202.70 | 80, 443, 8080 | 130 |
| 172.67.200.196 | 80, 443, 8080 | 131 |
| 172.67.223.46 | 80, 443, 8080 | 131 |
| 104.17.176.59 | 80, 443, 8080 | 133 |
| 104.19.2.75 | 80, 443, 8080 | 133 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9b02:4466:c934:d47f:8ca2:3e9d] | 80, 443, 8080 | 3 |
| [2606:4700:99e3:d031:99c1:dfb7:a5d2:3c1d] | 80, 443, 8080 | 3 |
| [2606:4700:9c6d:d606:e176:96ec:14e2:a0e2] | 80, 443, 8080 | 3 |
| [2606:4700:8392:9c0d:6b2b:a32b:5c6:8e94] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:9a05:802a:cedf:2a11:7caa] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:4466:c934:d47f:8ca2:3e9d] | 80, 443, 8080 | 3 |
| [2606:4700:99e3:d031:99c1:dfb7:a5d2:3c1d] | 80, 443, 8080 | 3 |
| [2606:4700:9c6d:d606:e176:96ec:14e2:a0e2] | 80, 443, 8080 | 3 |
| [2606:4700:8392:9c0d:6b2b:a32b:5c6:8e94] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:9a05:802a:cedf:2a11:7caa] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:4466:c934:d47f:8ca2:3e9d] | 80, 443, 8080 | 3 |
| [2606:4700:99e3:d031:99c1:dfb7:a5d2:3c1d] | 80, 443, 8080 | 3 |
| [2606:4700:9c6d:d606:e176:96ec:14e2:a0e2] | 80, 443, 8080 | 3 |
| [2606:4700:8392:9c0d:6b2b:a32b:5c6:8e94] | 80, 443, 8080 | 3 |
| [2606:4700:9b02:9a05:802a:cedf:2a11:7caa] | 80, 443, 8080 | 3 |

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
