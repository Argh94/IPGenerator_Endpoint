# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-03 23:45:11 +0330

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
| 162.159.36.61 | 80, 443, 8080 | 39 |
| 172.67.76.3 | 80, 443, 8080 | 42 |
| 172.67.78.30 | 80, 443, 8080 | 42 |
| 104.18.99.213 | 80, 443, 8080 | 130 |
| 104.18.99.213 | 80, 443, 8080 | 130 |
| 172.67.249.225 | 80, 443, 8080 | 131 |
| 172.67.239.92 | 80, 443, 8080 | 131 |
| 104.17.227.222 | 80, 443, 8080 | 132 |
| 104.17.227.222 | 80, 443, 8080 | 132 |
| 104.16.137.177 | 80, 443, 8080 | 133 |
| 104.17.141.213 | 80, 443, 8080 | 133 |
| 104.16.175.21 | 80, 443, 8080 | 133 |
| 104.16.137.177 | 80, 443, 8080 | 133 |
| 104.17.141.213 | 80, 443, 8080 | 133 |
| 104.16.175.21 | 80, 443, 8080 | 133 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:4407:45b7:416c:6131:51ab:20c9] | 80, 443, 8080 | 3 |
| [2606:4700:4407:45b7:416c:6131:51ab:20c9] | 80, 443, 8080 | 3 |
| [2606:4700:4407:45b7:416c:6131:51ab:20c9] | 80, 443, 8080 | 3 |
| [2606:4700:4407:ca2:b25e:27a0:c03a:7ded] | 80, 443, 8080 | 4 |
| [2606:4700:9ade:5a96:bb02:362d:7b9c:c2f7] | 80, 443, 8080 | 4 |
| [2606:4700:91ba:5b91:134a:1771:2466:8fca] | 80, 443, 8080 | 4 |
| [2606:4700:9ade:c5e8:bd17:b4a3:cc7c:9939] | 80, 443, 8080 | 4 |
| [2606:4700:4407:ca2:b25e:27a0:c03a:7ded] | 80, 443, 8080 | 4 |
| [2606:4700:9ade:5a96:bb02:362d:7b9c:c2f7] | 80, 443, 8080 | 4 |
| [2606:4700:91ba:5b91:134a:1771:2466:8fca] | 80, 443, 8080 | 4 |
| [2606:4700:9ade:c5e8:bd17:b4a3:cc7c:9939] | 80, 443, 8080 | 4 |
| [2606:4700:4407:ca2:b25e:27a0:c03a:7ded] | 80, 443, 8080 | 4 |
| [2606:4700:9ade:5a96:bb02:362d:7b9c:c2f7] | 80, 443, 8080 | 4 |
| [2606:4700:91ba:5b91:134a:1771:2466:8fca] | 80, 443, 8080 | 4 |
| [2606:4700:9ade:c5e8:bd17:b4a3:cc7c:9939] | 80, 443, 8080 | 4 |

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
