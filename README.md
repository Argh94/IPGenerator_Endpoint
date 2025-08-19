# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 Network Optimization with Top IPs

**IPOptimizer** fetches a list of optimized IPs (IPv4 and IPv6) with the lowest latency from [Hostmonit](https://hostmonit.com/) every 5 hours. These IPs are ideal for configuring proxies, VPNs, or improving network performance.

**Last Updated:** 2025-08-19 10:21:19 +0330

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
| 162.159.36.23 | 80, 443, 8080 | 57 |
| 172.67.185.49 | 80, 443, 8080 | 130 |
| 172.67.133.217 | 80, 443, 8080 | 130 |
| 172.67.241.173 | 80, 443, 8080 | 130 |
| 172.67.236.87 | 80, 443, 8080 | 131 |
| 104.18.233.72 | 80, 443, 8080 | 142 |
| 104.18.233.72 | 80, 443, 8080 | 142 |
| 104.19.241.95 | 80, 443, 8080 | 149 |
| 104.19.241.95 | 80, 443, 8080 | 149 |
| 104.17.185.91 | 80, 443, 8080 | 150 |
| 104.17.185.91 | 80, 443, 8080 | 150 |
| 104.21.82.1 | 80, 443, 8080 | 158 |
| 104.21.82.1 | 80, 443, 8080 | 158 |
| 104.18.136.57 | 80, 443, 8080 | 159 |
| 104.18.136.57 | 80, 443, 8080 | 159 |

### IPv6
| IP | Suggested Ports | Latency (ms) |
|----|------------------|--------------|
| [2606:4700:9a95:bd60:a388:5f6a:3f3a:d3fe] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:3ec6:da92:12b9:6db4:1004] | 80, 443, 8080 | 3 |
| [2606:4700:9a95:bd60:a388:5f6a:3f3a:d3fe] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:3ec6:da92:12b9:6db4:1004] | 80, 443, 8080 | 3 |
| [2606:4700:9a95:bd60:a388:5f6a:3f3a:d3fe] | 80, 443, 8080 | 3 |
| [2606:4700:9a91:3ec6:da92:12b9:6db4:1004] | 80, 443, 8080 | 3 |
| [2606:4700:4408:8e2f:cb7f:ff83:77f4:e2c] | 80, 443, 8080 | 4 |
| [2606:4700:4408:8e2f:cb7f:ff83:77f4:e2c] | 80, 443, 8080 | 4 |
| [2606:4700:4408:8e2f:cb7f:ff83:77f4:e2c] | 80, 443, 8080 | 4 |
| [2606:4700:83b7:d14f:fb74:b1a2:583f:1f19] | 80, 443, 8080 | 151 |
| [2606:4700:83b7:d14f:fb74:b1a2:583f:1f19] | 80, 443, 8080 | 151 |
| [2606:4700:83b7:d14f:fb74:b1a2:583f:1f19] | 80, 443, 8080 | 151 |
| [2606:4700:83b7:b8ae:6b17:f9:ad4d:ca98] | 80, 443, 8080 | 156 |
| [2606:4700:83b7:b8ae:6b17:f9:ad4d:ca98] | 80, 443, 8080 | 156 |
| [2606:4700:83b7:b8ae:6b17:f9:ad4d:ca98] | 80, 443, 8080 | 156 |

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
