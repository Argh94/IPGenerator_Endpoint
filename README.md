# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 بهینه‌سازی شبکه با IPهای برتر

**IPOptimizer** هر ۵ ساعت یک‌بار لیستی از IPهای بهینه (IPv4 و IPv6) با کمترین تأخیر را از [Hostmonit](https://hostmonit.com/) دریافت می‌کند. این IPها برای تنظیم پروکسی، VPN، یا بهبود عملکرد شبکه ایده‌آل هستند.

**آخرین به‌روزرسانی:** 2025-08-05 18:47:26 +0330

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
| 162.159.241.213 | 80, 443, 8080 | 56 |
| 172.67.74.40 | 80, 443, 8080 | 56 |
| 172.67.183.186 | 80, 443, 8080 | 134 |
| 172.67.198.215 | 80, 443, 8080 | 134 |
| 172.67.205.248 | 80, 443, 8080 | 136 |
| 104.25.36.186 | 80, 443, 8080 | 154 |
| 104.25.36.186 | 80, 443, 8080 | 154 |
| 104.17.219.124 | 80, 443, 8080 | 155 |
| 104.18.239.188 | 80, 443, 8080 | 155 |
| 104.17.219.124 | 80, 443, 8080 | 155 |
| 104.18.239.188 | 80, 443, 8080 | 155 |
| 104.19.133.228 | 80, 443, 8080 | 156 |
| 104.19.133.228 | 80, 443, 8080 | 156 |
| 104.21.42.183 | 80, 443, 8080 | 161 |
| 104.21.42.183 | 80, 443, 8080 | 161 |

### IPv6
| IP | پورت‌های پیشنهادی | تأخیر (ms) |
|----|-------------------|------------|
| [2606:4700:18:739c:51fd:1ac1:f5f3:b9cc] | 80, 443, 8080 | 9 |
| [2606:4700:18:739c:51fd:1ac1:f5f3:b9cc] | 80, 443, 8080 | 9 |
| [2606:4700:18:739c:51fd:1ac1:f5f3:b9cc] | 80, 443, 8080 | 9 |
| [2606:4700:90c9:ab2e:75e9:1086:87c6:cf9c] | 80, 443, 8080 | 16 |
| [2606:4700:90c9:7b47:c633:5fe6:bb38:e49b] | 80, 443, 8080 | 16 |
| [2606:4700:9ae7:e0d3:f315:1eaa:64da:8118] | 80, 443, 8080 | 16 |
| [2606:4700:9ad8:39b5:54c0:89bf:1a1d:7ae5] | 80, 443, 8080 | 16 |
| [2606:4700:90c9:ab2e:75e9:1086:87c6:cf9c] | 80, 443, 8080 | 16 |
| [2606:4700:90c9:7b47:c633:5fe6:bb38:e49b] | 80, 443, 8080 | 16 |
| [2606:4700:9ae7:e0d3:f315:1eaa:64da:8118] | 80, 443, 8080 | 16 |
| [2606:4700:9ad8:39b5:54c0:89bf:1a1d:7ae5] | 80, 443, 8080 | 16 |
| [2606:4700:90c9:ab2e:75e9:1086:87c6:cf9c] | 80, 443, 8080 | 16 |
| [2606:4700:90c9:7b47:c633:5fe6:bb38:e49b] | 80, 443, 8080 | 16 |
| [2606:4700:9ae7:e0d3:f315:1eaa:64da:8118] | 80, 443, 8080 | 16 |
| [2606:4700:9ad8:39b5:54c0:89bf:1a1d:7ae5] | 80, 443, 8080 | 16 |

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
