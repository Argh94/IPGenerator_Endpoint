# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 Network Optimization with Top IPs

**IPOptimizer** fetches a list of optimized IPs (IPv4 and IPv6) with the lowest latency from [Hostmonit](https://hostmonit.com/) every 5 hours. These IPs are ideal for configuring proxies, VPNs, or improving network performance.

**Last Updated:** 2025-08-16 10:20:00 +0330

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
| 141.101.121.249 | 80, 443, 8080 | 51 |
| 141.101.122.148 | 80, 443, 8080 | 51 |
| 141.101.120.246 | 80, 443, 8080 | 51 |
| 141.101.114.197 | 80, 443, 8080 | 51 |
| 141.101.114.245 | 80, 443, 8080 | 51 |
| 172.67.90.30 | 80, 443, 8080 | 56 |
| 162.159.238.149 | 80, 443, 8080 | 64 |
| 172.67.208.192 | 80, 443, 8080 | 130 |
| 172.67.213.135 | 80, 443, 8080 | 131 |
| 172.67.234.25 | 80, 443, 8080 | 132 |
| 104.19.57.5 | 80, 443, 8080 | 143 |
| 104.19.109.110 | 80, 443, 8080 | 147 |
| 104.21.231.245 | 80, 443, 8080 | 184 |
| 104.21.17.115 | 80, 443, 8080 | 185 |
| 104.18.31.100 | 80, 443, 8080 | 186 |

### IPv6
| IP | Suggested Ports | Latency (ms) |
|----|------------------|--------------|
| [2606:4700:9ae7:98e3:f81:1d4f:2af5:40bd] | 80, 443, 8080 | 3 |
| [2606:4700:9a97:b244:76a7:d7fd:71a7:58d4] | 80, 443, 8080 | 3 |
| [2606:4700:9ae7:98e3:f81:1d4f:2af5:40bd] | 80, 443, 8080 | 3 |
| [2606:4700:9a97:b244:76a7:d7fd:71a7:58d4] | 80, 443, 8080 | 3 |
| [2606:4700:9ae7:98e3:f81:1d4f:2af5:40bd] | 80, 443, 8080 | 3 |
| [2606:4700:9a97:b244:76a7:d7fd:71a7:58d4] | 80, 443, 8080 | 3 |
| [2606:4700:9644:7169:c146:3655:d3e5:be25] | 80, 443, 8080 | 4 |
| [2606:4700:9ae7:44d6:efb5:6f7c:57cd:be43] | 80, 443, 8080 | 4 |
| [2606:4700:9644:7169:c146:3655:d3e5:be25] | 80, 443, 8080 | 4 |
| [2606:4700:9ae7:44d6:efb5:6f7c:57cd:be43] | 80, 443, 8080 | 4 |
| [2606:4700:9644:7169:c146:3655:d3e5:be25] | 80, 443, 8080 | 4 |
| [2606:4700:9ae7:44d6:efb5:6f7c:57cd:be43] | 80, 443, 8080 | 4 |
| [2606:4700:23:8798:c783:ed76:b2a5:861] | 80, 443, 8080 | 5 |
| [2606:4700:23:8798:c783:ed76:b2a5:861] | 80, 443, 8080 | 5 |
| [2606:4700:23:8798:c783:ed76:b2a5:861] | 80, 443, 8080 | 5 |

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
