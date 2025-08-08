# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-08 18:44:44 +0330

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
| 162.159.36.177 | 80, 443, 8080 | 57 |
| 172.67.90.181 | 80, 443, 8080 | 57 |
| 162.159.133.142 | 80, 443, 8080 | 65 |
| 172.67.143.73 | 80, 443, 8080 | 130 |
| 172.67.253.20 | 80, 443, 8080 | 131 |
| 172.67.191.35 | 80, 443, 8080 | 131 |
| 104.16.80.218 | 80, 443, 8080 | 137 |
| 104.19.3.181 | 80, 443, 8080 | 137 |
| 104.19.69.147 | 80, 443, 8080 | 137 |
| 104.18.183.185 | 80, 443, 8080 | 143 |
| 104.17.218.184 | 80, 443, 8080 | 146 |
| 172.67.128.54 | 80, 443, 8080 | 224 |
| 141.101.122.120 | 80, 443, 8080 | 225 |
| 172.67.141.184 | 80, 443, 8080 | 226 |
| 172.67.100.223 | 80, 443, 8080 | 234 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:9ad9:11e6:87a6:7768:dbb7:a1ea] | 80, 443, 8080 | 3 |
| [2606:4700:9ad9:11e6:87a6:7768:dbb7:a1ea] | 80, 443, 8080 | 3 |
| [2606:4700:9ad9:11e6:87a6:7768:dbb7:a1ea] | 80, 443, 8080 | 3 |
| [2606:4700:3006:cbd7:c693:e917:38e1:c530] | 80, 443, 8080 | 4 |
| [2606:4700:9a64:e47:28da:8b82:8499:ef42] | 80, 443, 8080 | 4 |
| [2606:4700:9a64:b99e:8faf:dc42:a935:af15] | 80, 443, 8080 | 4 |
| [2606:4700:9aec:5d25:5313:faf1:6f77:3181] | 80, 443, 8080 | 4 |
| [2606:4700:3006:cbd7:c693:e917:38e1:c530] | 80, 443, 8080 | 4 |
| [2606:4700:9a64:e47:28da:8b82:8499:ef42] | 80, 443, 8080 | 4 |
| [2606:4700:9a64:b99e:8faf:dc42:a935:af15] | 80, 443, 8080 | 4 |
| [2606:4700:9aec:5d25:5313:faf1:6f77:3181] | 80, 443, 8080 | 4 |
| [2606:4700:3006:cbd7:c693:e917:38e1:c530] | 80, 443, 8080 | 4 |
| [2606:4700:9a64:e47:28da:8b82:8499:ef42] | 80, 443, 8080 | 4 |
| [2606:4700:9a64:b99e:8faf:dc42:a935:af15] | 80, 443, 8080 | 4 |
| [2606:4700:9aec:5d25:5313:faf1:6f77:3181] | 80, 443, 8080 | 4 |

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
