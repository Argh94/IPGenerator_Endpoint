# IPOptimizer

[![GitHub Actions](https://github.com/Argh94/IPOptimizer/workflows/IPOptimizer/badge.svg)](https://github.com/Argh94/IPOptimizer/actions)
[![PHP Version](https://img.shields.io/badge/PHP-8.0-blue)](https://www.php.net)
[![Update Frequency](https://img.shields.io/badge/Updates-Every%205%20Hours-green)](https://github.com/Argh94/IPOptimizer)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/Argh94/IPOptimizer)](https://github.com/Argh94/IPOptimizer/issues)

## 🚀 Network Optimization with Top IPs

**IPOptimizer** fetches a list of optimized IPs (IPv4 and IPv6) with the lowest latency from [Hostmonit](https://hostmonit.com/) every 5 hours. These IPs are ideal for configuring proxies, VPNs, or improving network performance.

**Last Updated:** 2025-08-26 10:22:08 +0330

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
| 198.41.208.186 | 80, 443, 8080 | 52 |
| 190.93.246.50 | 80, 443, 8080 | 53 |
| 198.41.209.192 | 80, 443, 8080 | 53 |
| 162.159.36.169 | 80, 443, 8080 | 56 |
| 162.159.138.169 | 80, 443, 8080 | 56 |
| 198.41.209.38 | 80, 443, 8080 | 57 |
| 172.67.129.31 | 80, 443, 8080 | 130 |
| 172.67.150.16 | 80, 443, 8080 | 131 |
| 172.67.203.221 | 80, 443, 8080 | 131 |
| 172.67.242.36 | 80, 443, 8080 | 149 |
| 104.18.80.70 | 80, 443, 8080 | 149 |
| 104.18.28.35 | 80, 443, 8080 | 154 |
| 141.101.120.147 | 80, 443, 8080 | 158 |
| 104.18.102.121 | 80, 443, 8080 | 159 |
| 104.16.193.163 | 80, 443, 8080 | 185 |

### IPv6
| IP | Suggested Ports | Latency (ms) |
|:---:|:---------------:|:------------:|
| [2606:4700:91b0:d195:979f:b046:b38a:36eb] | 80, 443, 8080 | 3 |
| [2606:4700:13a:9278:80e0:8b5f:22d8:8289] | 80, 443, 8080 | 3 |
| [2606:4700:839f:9a42:194e:c025:1a6f:d129] | 80, 443, 8080 | 3 |
| [2606:4700:91b8:e0d4:8bfa:f995:b399:4c19] | 80, 443, 8080 | 3 |
| [2606:4700:91b0:d195:979f:b046:b38a:36eb] | 80, 443, 8080 | 3 |
| [2606:4700:13a:9278:80e0:8b5f:22d8:8289] | 80, 443, 8080 | 3 |
| [2606:4700:839f:9a42:194e:c025:1a6f:d129] | 80, 443, 8080 | 3 |
| [2606:4700:91b8:e0d4:8bfa:f995:b399:4c19] | 80, 443, 8080 | 3 |
| [2606:4700:91b0:d195:979f:b046:b38a:36eb] | 80, 443, 8080 | 3 |
| [2606:4700:13a:9278:80e0:8b5f:22d8:8289] | 80, 443, 8080 | 3 |
| [2606:4700:839f:9a42:194e:c025:1a6f:d129] | 80, 443, 8080 | 3 |
| [2606:4700:91b8:e0d4:8bfa:f995:b399:4c19] | 80, 443, 8080 | 3 |
| [2606:4700:91b0:9e2d:b408:9958:702e:4d8a] | 80, 443, 8080 | 4 |
| [2606:4700:91b0:9e2d:b408:9958:702e:4d8a] | 80, 443, 8080 | 4 |
| [2606:4700:91b0:9e2d:b408:9958:702e:4d8a] | 80, 443, 8080 | 4 |

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
