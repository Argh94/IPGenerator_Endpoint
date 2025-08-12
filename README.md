# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-12 04:34:30 +0330

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
| 198.41.208.218 | 80, 443, 8080 | 50 |
| 198.41.209.14 | 80, 443, 8080 | 51 |
| 198.41.209.199 | 80, 443, 8080 | 52 |
| 198.41.209.135 | 80, 443, 8080 | 53 |
| 172.67.126.44 | 80, 443, 8080 | 56 |
| 172.67.95.34 | 80, 443, 8080 | 56 |
| 162.159.248.35 | 80, 443, 8080 | 56 |
| 172.67.81.0 | 80, 443, 8080 | 57 |
| 172.67.112.77 | 80, 443, 8080 | 57 |
| 162.159.129.243 | 80, 443, 8080 | 76 |
| 104.17.232.165 | 80, 443, 8080 | 128 |
| 104.16.141.114 | 80, 443, 8080 | 128 |
| 104.17.35.247 | 80, 443, 8080 | 129 |
| 104.17.128.235 | 80, 443, 8080 | 129 |
| 104.16.3.147 | 80, 443, 8080 | 133 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:8d77:6faa:d3e8:2ea4:dd43:eb66] | 80, 443, 8080 | 3 |
| [2606:4700:9c66:93e0:aeea:f581:a729:5f00] | 80, 443, 8080 | 3 |
| [2606:4700:9a6d:1ecc:27b5:9792:39b0:6ce3] | 80, 443, 8080 | 3 |
| [2606:4700:8d77:e787:e16d:2261:b002:cefb] | 80, 443, 8080 | 3 |
| [2606:4700:8d77:6faa:d3e8:2ea4:dd43:eb66] | 80, 443, 8080 | 3 |
| [2606:4700:9c66:93e0:aeea:f581:a729:5f00] | 80, 443, 8080 | 3 |
| [2606:4700:9a6d:1ecc:27b5:9792:39b0:6ce3] | 80, 443, 8080 | 3 |
| [2606:4700:8d77:e787:e16d:2261:b002:cefb] | 80, 443, 8080 | 3 |
| [2606:4700:8d77:6faa:d3e8:2ea4:dd43:eb66] | 80, 443, 8080 | 3 |
| [2606:4700:9c66:93e0:aeea:f581:a729:5f00] | 80, 443, 8080 | 3 |
| [2606:4700:9a6d:1ecc:27b5:9792:39b0:6ce3] | 80, 443, 8080 | 3 |
| [2606:4700:8d77:e787:e16d:2261:b002:cefb] | 80, 443, 8080 | 3 |
| [2606:4700:4406:4200:88dc:d158:9616:8fd2] | 80, 443, 8080 | 4 |
| [2606:4700:4406:4200:88dc:d158:9616:8fd2] | 80, 443, 8080 | 4 |
| [2606:4700:4406:4200:88dc:d158:9616:8fd2] | 80, 443, 8080 | 4 |

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
