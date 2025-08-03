# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-03 13:43:49 +0330

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
| 162.159.246.53 | 80, 443, 8080 | 43 |
| 104.18.209.194 | 80, 443, 8080 | 128 |
| 104.18.209.194 | 80, 443, 8080 | 128 |
| 172.67.241.67 | 80, 443, 8080 | 130 |
| 172.67.216.52 | 80, 443, 8080 | 130 |
| 172.67.211.207 | 80, 443, 8080 | 130 |
| 172.67.229.74 | 80, 443, 8080 | 131 |
| 104.16.163.156 | 80, 443, 8080 | 140 |
| 104.19.201.135 | 80, 443, 8080 | 140 |
| 104.16.163.156 | 80, 443, 8080 | 140 |
| 104.19.201.135 | 80, 443, 8080 | 140 |
| 104.19.104.216 | 80, 443, 8080 | 144 |
| 104.19.104.216 | 80, 443, 8080 | 144 |
| 104.27.62.81 | 80, 443, 8080 | 204 |
| 104.27.62.81 | 80, 443, 8080 | 204 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8d75:c28a:4d99:15d4:92ca:52a4] | 80, 443, 8080 | 3 |
| [2606:4700:3010:d830:c3c8:e475:a5a:88de] | 80, 443, 8080 | 3 |
| [2606:4700:90c8:360c:1adc:51d6:b7c:98d4] | 80, 443, 8080 | 3 |
| [2606:4700:8d75:c28a:4d99:15d4:92ca:52a4] | 80, 443, 8080 | 3 |
| [2606:4700:3010:d830:c3c8:e475:a5a:88de] | 80, 443, 8080 | 3 |
| [2606:4700:90c8:360c:1adc:51d6:b7c:98d4] | 80, 443, 8080 | 3 |
| [2606:4700:8d75:c28a:4d99:15d4:92ca:52a4] | 80, 443, 8080 | 3 |
| [2606:4700:3010:d830:c3c8:e475:a5a:88de] | 80, 443, 8080 | 3 |
| [2606:4700:90c8:360c:1adc:51d6:b7c:98d4] | 80, 443, 8080 | 3 |
| [2606:4700:3017:2d8a:4bea:5123:a5dd:d5d0] | 80, 443, 8080 | 4 |
| [2606:4700:3017:5a2d:faf7:826d:6be9:defb] | 80, 443, 8080 | 4 |
| [2606:4700:3017:2d8a:4bea:5123:a5dd:d5d0] | 80, 443, 8080 | 4 |
| [2606:4700:3017:5a2d:faf7:826d:6be9:defb] | 80, 443, 8080 | 4 |
| [2606:4700:3017:2d8a:4bea:5123:a5dd:d5d0] | 80, 443, 8080 | 4 |
| [2606:4700:3017:5a2d:faf7:826d:6be9:defb] | 80, 443, 8080 | 4 |

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
