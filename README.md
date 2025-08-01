# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-01 18:45:17 +0330

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
| 172.67.105.167 | 80, 443, 8080 | 39 |
| 172.67.118.252 | 80, 443, 8080 | 40 |
| 172.67.175.37 | 80, 443, 8080 | 130 |
| 172.67.233.236 | 80, 443, 8080 | 130 |
| 172.67.211.36 | 80, 443, 8080 | 130 |
| 104.19.219.138 | 80, 443, 8080 | 143 |
| 104.19.219.138 | 80, 443, 8080 | 143 |
| 104.19.67.91 | 80, 443, 8080 | 144 |
| 104.19.67.91 | 80, 443, 8080 | 144 |
| 104.19.105.143 | 80, 443, 8080 | 147 |
| 104.19.105.143 | 80, 443, 8080 | 147 |
| 104.18.25.235 | 80, 443, 8080 | 154 |
| 104.18.25.235 | 80, 443, 8080 | 154 |
| 172.67.210.103 | 80, 443, 8080 | 159 |
| 172.67.210.103 | 80, 443, 8080 | 159 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8d75:a6de:d46e:47b2:6632:b4e3] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:a92e:568b:5cf8:8294:935c] | 80, 443, 8080 | 3 |
| [2606:4700:8d75:a6de:d46e:47b2:6632:b4e3] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:a92e:568b:5cf8:8294:935c] | 80, 443, 8080 | 3 |
| [2606:4700:8d75:a6de:d46e:47b2:6632:b4e3] | 80, 443, 8080 | 3 |
| [2606:4700:8d7b:a92e:568b:5cf8:8294:935c] | 80, 443, 8080 | 3 |
| [2606:4700:8d75:13f2:bd23:4b49:edf8:47b4] | 80, 443, 8080 | 4 |
| [2606:4700:9646:5fb9:b47e:5f9a:7bf2:2d21] | 80, 443, 8080 | 4 |
| [2606:4700:8dd5:ba4b:a2f9:4f1:2c92:601] | 80, 443, 8080 | 4 |
| [2606:4700:8d75:13f2:bd23:4b49:edf8:47b4] | 80, 443, 8080 | 4 |
| [2606:4700:9646:5fb9:b47e:5f9a:7bf2:2d21] | 80, 443, 8080 | 4 |
| [2606:4700:8dd5:ba4b:a2f9:4f1:2c92:601] | 80, 443, 8080 | 4 |
| [2606:4700:8d75:13f2:bd23:4b49:edf8:47b4] | 80, 443, 8080 | 4 |
| [2606:4700:9646:5fb9:b47e:5f9a:7bf2:2d21] | 80, 443, 8080 | 4 |
| [2606:4700:8dd5:ba4b:a2f9:4f1:2c92:601] | 80, 443, 8080 | 4 |

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
