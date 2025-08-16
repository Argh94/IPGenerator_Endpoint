# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 Network Optimization with Top IPs

**IPOptimizer** fetches a list of optimized IPs (IPv4 and IPv6) with the lowest latency from [Hostmonit](https://hostmonit.com/) every 5 hours. These IPs are ideal for configuring proxies, VPNs, or improving network performance.

**Last Updated:** 2025-08-17 00:08:15 +0330

**JSON Files**: The `ipv4.json`, `ipv6.json`, and `export.json` files are available in the [Releases section](https://github.com/Argh94/IPOptimizer/releases).

## ✨ Features
- 📡 **Low-Latency IPs**: Sorted by lowest latency.
- 🔍 **Suggested Ports**: Open ports (80, 443, 8080) are automatically checked.
- ⏰ **Regular Updates**: Every 5 hours via GitHub Actions.
- 📄 **JSON Outputs**: Data is stored in the Releases section (`ipv4.json`, `ipv6.json`, `export.json`).

## 📋 Optimized IPs

**Note:** The displayed ports have been checked by the server, but they may vary depending on your network. For verification, use [YouGetSignal](https://www.yougetsignal.com/tools/open-ports/) (IPv4) or [Nmap](https://nmap.org/) (IPv6).

### IPv4
| IP | Suggested Ports | Latency (ms) |
|----|------------------|--------------|
| 172.67.98.236 | 80, 443, 8080 | 56 |
| 198.41.222.42 | 80, 443, 8080 | 56 |
| 172.67.64.19 | 80, 443, 8080 | 57 |
| 172.64.78.113 | 80, 443, 8080 | 57 |
| 104.19.26.70 | 80, 443, 8080 | 129 |
| 104.19.26.70 | 80, 443, 8080 | 129 |
| 172.67.247.25 | 80, 443, 8080 | 130 |
| 104.16.78.79 | 80, 443, 8080 | 131 |
| 104.16.78.79 | 80, 443, 8080 | 131 |
| 104.19.102.234 | 80, 443, 8080 | 132 |
| 104.19.33.0 | 80, 443, 8080 | 132 |
| 104.19.102.234 | 80, 443, 8080 | 132 |
| 104.19.33.0 | 80, 443, 8080 | 132 |
| 104.17.231.112 | 80, 443, 8080 | 139 |
| 104.17.231.112 | 80, 443, 8080 | 139 |

### IPv6
| IP | Suggested Ports | Latency (ms) |
|----|------------------|--------------|
| [2606:4700:8:9cd:bbc7:5491:8b81:bbcd] | 80, 443, 8080 | 4 |
| [2606:4700:8:45ab:ca93:146b:95a1:8c7] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:5f90:f4c8:86c:e177:4e5d] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:28:8602:71ad:6d06:eb0] | 80, 443, 8080 | 4 |
| [2606:4700:90da:1291:a004:a598:d15d:5af0] | 80, 443, 8080 | 4 |
| [2606:4700:8:9cd:bbc7:5491:8b81:bbcd] | 80, 443, 8080 | 4 |
| [2606:4700:8:45ab:ca93:146b:95a1:8c7] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:5f90:f4c8:86c:e177:4e5d] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:28:8602:71ad:6d06:eb0] | 80, 443, 8080 | 4 |
| [2606:4700:90da:1291:a004:a598:d15d:5af0] | 80, 443, 8080 | 4 |
| [2606:4700:8:9cd:bbc7:5491:8b81:bbcd] | 80, 443, 8080 | 4 |
| [2606:4700:8:45ab:ca93:146b:95a1:8c7] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:5f90:f4c8:86c:e177:4e5d] | 80, 443, 8080 | 4 |
| [2606:4700:9ae8:28:8602:71ad:6d06:eb0] | 80, 443, 8080 | 4 |
| [2606:4700:90da:1291:a004:a598:d15d:5af0] | 80, 443, 8080 | 4 |

## 🛠️ Installation and Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Argh94/IPOptimizer.git
   ```
2. **PHP Setup**:
   - Install PHP 8.0 or higher.
   - Set the Hostmonit API key in the `HOSTMONIT_API_KEY` environment variable:
     ```bash
     export HOSTMONIT_API_KEY="your-api-key"
     ```
3. **Run the Script**:
   ```bash
   php scripts/fetch_ips.php
   ```
4. **Check Output**:
   - JSON files are available in the [Releases section](https://github.com/Argh94/IPOptimizer/releases).
   - IP list in `README.md`.

## 📬 Support
- 🐛 **Report Issues**: [Issues](https://github.com/Argh94/IPOptimizer/issues)
- 📧 **Contact**: [ircfspace@gmail.com](mailto:ircfspace@gmail.com)

## 📄 License
This project is licensed under the [MIT License](https://github.com/Argh94/HandWave/blob/main/LICENCE).
