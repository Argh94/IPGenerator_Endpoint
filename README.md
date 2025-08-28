# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 Network Optimization with Top IPs

**IPOptimizer** fetches a list of optimized IPs (IPv4 and IPv6) with the lowest latency from [Hostmonit](https://hostmonit.com/) every 5 hours. These IPs are ideal for configuring proxies, VPNs, or improving network performance.

**Last Updated:** 2025-08-28 10:20:12 +0330

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
|:---:|:---------------:|:------------:|
| 172.64.68.47 | 80, 443, 8080 | 53 |
| 172.64.68.165 | 80, 443, 8080 | 56 |
| 172.67.111.217 | 80, 443, 8080 | 56 |
| 172.67.70.163 | 80, 443, 8080 | 57 |
| 198.41.209.187 | 80, 443, 8080 | 58 |
| 198.41.208.216 | 80, 443, 8080 | 61 |
| 198.41.208.232 | 80, 443, 8080 | 62 |
| 162.159.136.154 | 80, 443, 8080 | 78 |
| 172.67.186.118 | 80, 443, 8080 | 131 |
| 172.67.188.77 | 80, 443, 8080 | 131 |
| 104.19.195.64 | 80, 443, 8080 | 134 |
| 104.17.103.253 | 80, 443, 8080 | 134 |
| 104.19.218.8 | 80, 443, 8080 | 140 |
| 104.18.66.214 | 80, 443, 8080 | 148 |
| 104.21.230.172 | 80, 443, 8080 | 149 |

### IPv6
| IP | Suggested Ports | Latency (ms) |
|:---:|:---------------:|:------------:|
| [2606:4700:9ae6:4ac1:96f5:f3d3:4b4a:d0d2] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:6d3c:c386:53c4:3ddc:2a13] | 80, 443, 8080 | 3 |
| [2606:4700:9a9a:e3a5:f050:89ce:947b:47e2] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:4ac1:96f5:f3d3:4b4a:d0d2] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:6d3c:c386:53c4:3ddc:2a13] | 80, 443, 8080 | 3 |
| [2606:4700:9a9a:e3a5:f050:89ce:947b:47e2] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:4ac1:96f5:f3d3:4b4a:d0d2] | 80, 443, 8080 | 3 |
| [2606:4700:9ae6:6d3c:c386:53c4:3ddc:2a13] | 80, 443, 8080 | 3 |
| [2606:4700:9a9a:e3a5:f050:89ce:947b:47e2] | 80, 443, 8080 | 3 |
| [2606:4700:d0:f884:5ec1:de3c:6937:d7bd] | 80, 443, 8080 | 4 |
| [2606:4700:90de:2dc3:19d9:4367:7f32:a80f] | 80, 443, 8080 | 4 |
| [2606:4700:d0:f884:5ec1:de3c:6937:d7bd] | 80, 443, 8080 | 4 |
| [2606:4700:90de:2dc3:19d9:4367:7f32:a80f] | 80, 443, 8080 | 4 |
| [2606:4700:d0:f884:5ec1:de3c:6937:d7bd] | 80, 443, 8080 | 4 |
| [2606:4700:90de:2dc3:19d9:4367:7f32:a80f] | 80, 443, 8080 | 4 |

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
