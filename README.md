# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-02 18:43:13 +0330

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
| 162.159.247.86 | 80, 443, 8080 | 39 |
| 172.67.95.181 | 80, 443, 8080 | 40 |
| 172.67.95.154 | 80, 443, 8080 | 42 |
| 172.67.249.40 | 80, 443, 8080 | 130 |
| 172.67.170.71 | 80, 443, 8080 | 131 |
| 104.18.240.113 | 80, 443, 8080 | 137 |
| 104.18.240.113 | 80, 443, 8080 | 137 |
| 104.17.131.102 | 80, 443, 8080 | 149 |
| 104.17.131.102 | 80, 443, 8080 | 149 |
| 104.16.112.119 | 80, 443, 8080 | 150 |
| 104.16.112.119 | 80, 443, 8080 | 150 |
| 104.17.93.190 | 80, 443, 8080 | 157 |
| 104.17.93.190 | 80, 443, 8080 | 157 |
| 104.18.97.118 | 80, 443, 8080 | 181 |
| 104.18.97.118 | 80, 443, 8080 | 181 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:91be:539e:9557:3f96:8086:afa5] | 80, 443, 8080 | 3 |
| [2606:4700:91be:2c24:35eb:cf5f:49c0:986e] | 80, 443, 8080 | 3 |
| [2606:4700:91be:539e:9557:3f96:8086:afa5] | 80, 443, 8080 | 3 |
| [2606:4700:91be:2c24:35eb:cf5f:49c0:986e] | 80, 443, 8080 | 3 |
| [2606:4700:91be:539e:9557:3f96:8086:afa5] | 80, 443, 8080 | 3 |
| [2606:4700:91be:2c24:35eb:cf5f:49c0:986e] | 80, 443, 8080 | 3 |
| [2606:4700:8cad:44a5:9195:acc1:8664:a1e5] | 80, 443, 8080 | 4 |
| [2606:4700:8cad:44a5:9195:acc1:8664:a1e5] | 80, 443, 8080 | 4 |
| [2606:4700:8cad:44a5:9195:acc1:8664:a1e5] | 80, 443, 8080 | 4 |
| [2606:4700:83b1:5086:cce7:b6b5:c0bf:6a7e] | 80, 443, 8080 | 144 |
| [2606:4700:83b1:5086:cce7:b6b5:c0bf:6a7e] | 80, 443, 8080 | 144 |
| [2606:4700:83b1:5086:cce7:b6b5:c0bf:6a7e] | 80, 443, 8080 | 144 |
| [2606:4700:83b1:22c9:3717:4552:33c3:68cc] | 80, 443, 8080 | 156 |
| [2606:4700:83b1:22c9:3717:4552:33c3:68cc] | 80, 443, 8080 | 156 |
| [2606:4700:83b1:22c9:3717:4552:33c3:68cc] | 80, 443, 8080 | 156 |

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
