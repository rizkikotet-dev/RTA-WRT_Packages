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
    <img src="https://img.shields.io/badge/4456-packages-blue?style=flat-square" alt="4456 packages">
  </td>
  <td align="center">
    <img src="https://img.shields.io/badge/44-architectures-green?style=flat-square" alt="44 architectures">
  </td>
  <td align="center">
    <img src="https://img.shields.io/badge/3-branches-orange?style=flat-square" alt="3 branches">
  </td>
  <td align="center">
    <img src="https://img.shields.io/badge/818MB-size-red?style=flat-square" alt="818MB">
  </td>
</tr>
</table>

> 🕐 **Last updated**: 2025-06-22 18:46:41 UTC

## 🌿 Supported OpenWRT Versions

### ![Stable](https://img.shields.io/badge/23.05-Stable-green?style=flat-square)

| Architecture | Packages | Status |
|--------------|----------|--------|
| `aarch64_cortex-a53-openwrt` | 104 | ✅ Available |
| `aarch64_cortex-a72-openwrt` | 104 | ✅ Available |
| `aarch64_generic-openwrt` | 104 | ✅ Available |
| `arm_cortex-a15_neon-vfpv4-openwrt` | 104 | ✅ Available |
| `arm_cortex-a5_vfpv4-openwrt` | 104 | ✅ Available |
| `arm_cortex-a7_neon-vfpv4-openwrt` | 104 | ✅ Available |
| `arm_cortex-a8_vfpv3-openwrt` | 104 | ✅ Available |
| `arm_cortex-a9-openwrt` | 104 | ✅ Available |
| `arm_cortex-a9_neon-openwrt` | 104 | ✅ Available |
| `arm_cortex-a9_vfpv3-d16-openwrt` | 104 | ✅ Available |
| `i386_pentium4-openwrt` | 102 | ✅ Available |
| `mips64_octeonplus-openwrt` | 102 | ✅ Available |
| `mips_24kc-openwrt` | 102 | ✅ Available |
| `mips_4kec-openwrt` | 69 | ✅ Available |
| `mips_mips32-openwrt` | 102 | ✅ Available |
| `mipsel_24kc_24kf-openwrt` | 102 | ✅ Available |
| `mipsel_74kc-openwrt` | 102 | ✅ Available |
| `mipsel_mips32-openwrt` | 102 | ✅ Available |
| `x86_64-openwrt` | 102 | ✅ Available |

### ![Stable](https://img.shields.io/badge/24.10-Stable-green?style=flat-square)

| Architecture | Packages | Status |
|--------------|----------|--------|
| `aarch64_cortex-a53-openwrt` | 104 | ✅ Available |
| `aarch64_cortex-a72-openwrt` | 104 | ✅ Available |
| `aarch64_cortex-a76-openwrt` | 104 | ✅ Available |
| `aarch64_generic-openwrt` | 104 | ✅ Available |
| `arm_cortex-a15_neon-vfpv4-openwrt` | 104 | ✅ Available |
| `arm_cortex-a5_vfpv4-openwrt` | 104 | ✅ Available |
| `arm_cortex-a7_neon-vfpv4-openwrt` | 104 | ✅ Available |
| `arm_cortex-a8_vfpv3-openwrt` | 104 | ✅ Available |
| `arm_cortex-a9-openwrt` | 104 | ✅ Available |
| `arm_cortex-a9_neon-openwrt` | 104 | ✅ Available |
| `arm_cortex-a9_vfpv3-d16-openwrt` | 104 | ✅ Available |
| `i386_pentium4-openwrt` | 102 | ✅ Available |
| `mips64_octeonplus-openwrt` | 102 | ✅ Available |
| `mips_24kc-openwrt` | 102 | ✅ Available |
| `mips_4kec-openwrt` | 69 | ✅ Available |
| `mips_mips32-openwrt` | 102 | ✅ Available |
| `mipsel_24kc-openwrt` | 102 | ✅ Available |
| `mipsel_24kc_24kf-openwrt` | 102 | ✅ Available |
| `mipsel_74kc-openwrt` | 102 | ✅ Available |
| `mipsel_mips32-openwrt` | 102 | ✅ Available |
| `x86_64-openwrt` | 102 | ✅ Available |

### ![SNAPSHOT](https://img.shields.io/badge/SNAPSHOT-Development-red?style=flat-square)

| Architecture | Packages | Status |
|--------------|----------|--------|
| `aarch64_cortex-a76` | 104 | ✅ Available |
| `arm_cortex-a9_vfpv3-d16` | 92 | ✅ Available |
| `mips_mips32` | 102 | ✅ Available |
| `mipsel_24kc` | 102 | ✅ Available |

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

### Method 3: Batch Installation Script

```bash
#!/bin/bash
# Auto-detect architecture and install packages
ARCH=$(opkg print-architecture | awk 'NR==2{print $2}')
BRANCH="openwrt-23.05"  # or openwrt-24.10, SNAPSHOT

# Add repository
echo "src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/$BRANCH/$ARCH" > /etc/opkg/customfeeds.conf

# Update and install
opkg update
opkg list | grep custom_packages
```

## 🔧 Architecture Detection

Not sure about your architecture? Run this on your OpenWRT device:

```bash
opkg print-architecture | head -5
cat /proc/cpuinfo | grep "model name\|cpu model\|Hardware"
```

## 📋 Available Packages by Category

<details>
<summary>🔍 <strong>Click to view package categories</strong></summary>
<br>

| Category | Description | Example Packages |
|----------|-------------|------------------|
| 🌐 **Network** | Networking tools and protocols | `curl`, `wget`, `iperf3` |
| 🔒 **Security** | Security and encryption tools | `openssl`, `dropbear`, `wireguard` |
| 🛠️ **System** | System utilities and tools | `htop`, `nano`, `rsync` |
| 📡 **Wireless** | WiFi and wireless utilities | `hostapd`, `wpa-supplicant` |
| 💾 **Storage** | File system and storage tools | `block-mount`, `kmod-fs-ext4` |
| 🔌 **Hardware** | Hardware drivers and support | `kmod-usb-storage`, `kmod-i2c` |

</details>

## 🛡️ Quality Assurance

- ✅ **Automated Testing**: All packages undergo validation
- 🔄 **Weekly Builds**: Fresh packages every week
- 📊 **Build Monitoring**: Failed builds are tracked and fixed
- 🏷️ **Version Tracking**: Clear versioning and changelog

## 🤝 Contributing

Want to add your packages? Here's how:

1. **Fork** this repository
2. **Add** your packages to the `packages/` directory
3. **Test** locally with OpenWRT SDK
4. **Submit** a pull request

### Package Structure
```
packages/
├── your-package/
│   ├── Makefile
│   ├── files/
│   └── patches/
```

## 🐛 Troubleshooting

<details>
<summary>❓ <strong>Common Issues & Solutions</strong></summary>

### Package Installation Fails
```bash
# Clear opkg cache and retry
rm -rf /tmp/opkg-lists/*
opkg update
opkg install [package_name]
```

### Architecture Mismatch
```bash
# Check your device architecture
opkg print-architecture
# Use the correct architecture in repository URL
```

### Repository Not Found
```bash
# Verify repository URL is correct
cat /etc/opkg/customfeeds.conf
```

</details>

## 📈 Build Status & Monitoring

<div align="center">
  <a href="../../actions">
    <img src="https://img.shields.io/github/actions/workflow/status/rizkikotet-dev/RTA-WRT_Packages/build.yml?branch=main&style=for-the-badge&logo=github-actions" alt="Build Status">
  </a>
  <a href="../../releases">
    <img src="https://img.shields.io/github/v/release/rizkikotet-dev/RTA-WRT_Packages?style=for-the-badge&logo=github" alt="Latest Release">
  </a>
  <a href="../../commits/main">
    <img src="https://img.shields.io/github/last-commit/rizkikotet-dev/RTA-WRT_Packages?style=for-the-badge&logo=git" alt="Last Commit">
  </a>
</div>

## 📞 Support & Community

- 🐛 **Bug Reports**: [Create an Issue](../../issues/new?template=bug_report.md)
- 💡 **Feature Requests**: [Request Feature](../../issues/new?template=feature_request.md)
- 💬 **Discussions**: [Join Discussion](../../discussions)
- 📧 **Contact**: [Email Support](mailto:support@example.com)

## 📄 License & Legal

This repository contains packages from various sources. Each package maintains its original license.

- 📜 **Repository License**: MIT
- ⚖️ **Package Licenses**: Varies (see individual packages)
- 🔒 **Privacy Policy**: No personal data collected

---

<div align="center">
  <h3>🌟 Star this repository if it helps you!</h3>
  <p>
    <a href="../../stargazers">⭐ Star</a> •
    <a href="../../network/members">🍴 Fork</a> •
    <a href="../../issues">🐛 Report Bug</a> •
    <a href="../../discussions">💬 Discuss</a>
  </p>
</div>

<div align="center">
  <sub>Built with ❤️ using GitHub Actions • Powered by OpenWRT | RizkiKotet</sub>
</div>
