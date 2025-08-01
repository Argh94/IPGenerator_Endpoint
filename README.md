# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-01 23:45:22 +0330

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
| 172.67.74.150 | 80, 443, 8080 | 38 |
| 172.64.84.134 | 80, 443, 8080 | 40 |
| 104.19.121.241 | 80, 443, 8080 | 129 |
| 104.18.227.240 | 80, 443, 8080 | 129 |
| 104.19.121.241 | 80, 443, 8080 | 129 |
| 104.18.227.240 | 80, 443, 8080 | 129 |
| 172.67.205.203 | 80, 443, 8080 | 130 |
| 172.67.236.3 | 80, 443, 8080 | 130 |
| 172.67.247.206 | 80, 443, 8080 | 130 |
| 104.17.220.199 | 80, 443, 8080 | 132 |
| 104.17.220.199 | 80, 443, 8080 | 132 |
| 104.19.184.232 | 80, 443, 8080 | 133 |
| 104.17.143.134 | 80, 443, 8080 | 133 |
| 104.19.184.232 | 80, 443, 8080 | 133 |
| 104.17.143.134 | 80, 443, 8080 | 133 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:90d9:c38f:c442:7457:cfdc:ba8c] | 80, 443, 8080 | 3 |
| [2606:4700:12:5bc5:46b6:14ce:c64d:6498] | 80, 443, 8080 | 3 |
| [2606:4700:90d9:c38f:c442:7457:cfdc:ba8c] | 80, 443, 8080 | 3 |
| [2606:4700:12:5bc5:46b6:14ce:c64d:6498] | 80, 443, 8080 | 3 |
| [2606:4700:90d9:c38f:c442:7457:cfdc:ba8c] | 80, 443, 8080 | 3 |
| [2606:4700:12:5bc5:46b6:14ce:c64d:6498] | 80, 443, 8080 | 3 |
| [2606:4700:9c6c:60f6:4e6d:9c9d:906:cec2] | 80, 443, 8080 | 4 |
| [2606:4700:9a63:b100:4e73:b3ef:4882:3f77] | 80, 443, 8080 | 4 |
| [2606:4700:9a63:c65:5ca5:464c:828:d5a9] | 80, 443, 8080 | 4 |
| [2606:4700:9c6c:60f6:4e6d:9c9d:906:cec2] | 80, 443, 8080 | 4 |
| [2606:4700:9a63:b100:4e73:b3ef:4882:3f77] | 80, 443, 8080 | 4 |
| [2606:4700:9a63:c65:5ca5:464c:828:d5a9] | 80, 443, 8080 | 4 |
| [2606:4700:9c6c:60f6:4e6d:9c9d:906:cec2] | 80, 443, 8080 | 4 |
| [2606:4700:9a63:b100:4e73:b3ef:4882:3f77] | 80, 443, 8080 | 4 |
| [2606:4700:9a63:c65:5ca5:464c:828:d5a9] | 80, 443, 8080 | 4 |

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
