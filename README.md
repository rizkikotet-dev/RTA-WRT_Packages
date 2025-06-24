# 🚀 OpenWRT Custom Packages Repository

<div align="center">
  <img src="https://img.shields.io/badge/OpenWRT-Packages-blue?style=for-the-badge&logo=openwrt" alt="OpenWRT Packages">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Auto--Updated-Weekly-informational?style=for-the-badge" alt="Auto Updated">
</div>

<div align="center">
  <h3>🎯 Pre-built packages for multiple OpenWRT versions and architectures</h3>
  <p><em>Automated builds • Quality assured • Always up-to-date</em></p>
</div>

---

## 📊 Repository Statistics

<table>
  <tr>
    <td align="center"><strong>📦 Total Packages</strong></td>
    <td align="center"><strong>🏗️ Architectures</strong></td>
    <td align="center"><strong>🌿 Branches</strong></td>
    <td align="center"><strong>💾 Repository Size</strong></td>
  </tr>
  <tr>
    <td align="center">
    <img src="https://img.shields.io/badge/5022-packages-blue?style=flat-square" alt="5022 packages">
  </td>
  <td align="center">
    <img src="https://img.shields.io/badge/16-architectures-green?style=flat-square" alt="16 architectures">
  </td>
  <td align="center">
    <img src="https://img.shields.io/badge/3-branches-orange?style=flat-square" alt="3 branches">
  </td>
  <td align="center">
    <img src="https://img.shields.io/badge/409MB-size-red?style=flat-square" alt="409MB">
  </td>
</tr>
</table>

> 🕐 **Last updated**: 2025-06-24 18:13:04 UTC

## 🌿 Supported OpenWRT Versions

### ![Stable](https://img.shields.io/badge/23.05-Stable-green?style=flat-square)

| Architecture | Packages | Status |
|--------------|----------|--------|
| `aarch64_cortex-a53` | 336 | ✅ Available |
| `aarch64_cortex-a72` | 336 | ✅ Available |
| `aarch64_cortex-a76` | 336 | ✅ Available |
| `aarch64_generic` | 336 | ✅ Available |
| `openwrt-23.05` | 336 | ✅ Available |
| `x86_64` | 331 | ✅ Available |

### ![Stable](https://img.shields.io/badge/24.10-Stable-green?style=flat-square)

| Architecture | Packages | Status |
|--------------|----------|--------|
| `aarch64_cortex-a53` | 336 | ✅ Available |
| `aarch64_cortex-a72` | 336 | ✅ Available |
| `aarch64_cortex-a76` | 336 | ✅ Available |
| `aarch64_generic` | 336 | ✅ Available |
| `openwrt-24.10` | 336 | ✅ Available |
| `x86_64` | 331 | ✅ Available |

### ![SNAPSHOT](https://img.shields.io/badge/SNAPSHOT-Development-red?style=flat-square)

| Architecture | Packages | Status |
|--------------|----------|--------|
| `aarch64_cortex-a76` | 333 | ✅ Available |
| `aarch64_generic` | 336 | ✅ Available |
| `x86_64` | 331 | ✅ Available |

## 🚀 Quick Start

### Method 1: Add Repository Source

```bash
# Add custom repository (replace [BRANCH] and [ARCH] with your values)
echo "src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/[BRANCH]/[ARCH]" >> /etc/opkg/customfeeds.conf

# Update package lists
opkg update

# Install packages
opkg install [package_name]
```

### Method 2: Direct Download

Browse packages directly at: [📂 Package Browser](../../tree/releases/packages)

### Method 3: Auto-detect Architecture

```bash
#!/bin/bash
# Auto-detect architecture and install packages
ARCH=$(opkg print-architecture | awk 'NR==2{print $2}')
BRANCH="23.05"  # or 24.10, SNAPSHOT

# Add repository
echo "src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/$BRANCH/$ARCH" > /etc/opkg/customfeeds.conf

# Update and install
opkg update
opkg list | grep custom_packages
```

## 📞 Support

- 🐛 **Bug Reports**: [Create an Issue](../../issues/new)
- 💡 **Feature Requests**: [Request Feature](../../issues/new)
- 📧 **Questions**: [Discussions](../../discussions)

---

<div align="center">
  <sub>Built with ❤️ using GitHub Actions • Powered by OpenWRT</sub>
</div>
