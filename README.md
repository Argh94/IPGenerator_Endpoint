# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-09 04:34:57 +0330

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
| 141.101.120.189 | 80, 443, 8080 | 56 |
| 172.64.89.78 | 80, 443, 8080 | 56 |
| 162.159.130.95 | 80, 443, 8080 | 63 |
| 104.16.99.122 | 80, 443, 8080 | 130 |
| 172.67.221.168 | 80, 443, 8080 | 130 |
| 172.67.131.142 | 80, 443, 8080 | 131 |
| 172.67.192.132 | 80, 443, 8080 | 131 |
| 104.17.55.219 | 80, 443, 8080 | 133 |
| 104.16.9.229 | 80, 443, 8080 | 133 |
| 104.16.171.190 | 80, 443, 8080 | 133 |
| 104.16.173.180 | 80, 443, 8080 | 136 |
| 172.67.123.254 | 80, 443, 8080 | 205 |
| 172.67.114.250 | 80, 443, 8080 | 206 |
| 172.67.94.174 | 80, 443, 8080 | 209 |
| 172.67.177.128 | 80, 443, 8080 | 210 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:3025:4c18:b21a:dfc9:cbd5:afe1] | 80, 443, 8080 | 9 |
| [2606:4700:3025:52c9:23f8:91df:e9e9:c9c8] | 80, 443, 8080 | 9 |
| [2606:4700:3019:6f13:e6ff:ecb0:621e:f544] | 80, 443, 8080 | 9 |
| [2606:4700:3025:4c18:b21a:dfc9:cbd5:afe1] | 80, 443, 8080 | 9 |
| [2606:4700:3025:52c9:23f8:91df:e9e9:c9c8] | 80, 443, 8080 | 9 |
| [2606:4700:3019:6f13:e6ff:ecb0:621e:f544] | 80, 443, 8080 | 9 |
| [2606:4700:3025:4c18:b21a:dfc9:cbd5:afe1] | 80, 443, 8080 | 9 |
| [2606:4700:3025:52c9:23f8:91df:e9e9:c9c8] | 80, 443, 8080 | 9 |
| [2606:4700:3019:6f13:e6ff:ecb0:621e:f544] | 80, 443, 8080 | 9 |
| [2606:4700:3019:fe61:9783:b21d:41ab:85aa] | 80, 443, 8080 | 10 |
| [2606:4700:3019:fe61:9783:b21d:41ab:85aa] | 80, 443, 8080 | 10 |
| [2606:4700:3019:fe61:9783:b21d:41ab:85aa] | 80, 443, 8080 | 10 |
| [2606:4700:91b0:db60:b5e1:19f7:1725:e631] | 80, 443, 8080 | 16 |
| [2606:4700:91b0:db60:b5e1:19f7:1725:e631] | 80, 443, 8080 | 16 |
| [2606:4700:91b0:db60:b5e1:19f7:1725:e631] | 80, 443, 8080 | 16 |

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
