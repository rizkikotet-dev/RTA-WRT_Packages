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

## 🌿 Supported OpenWRT Versions

### ![Stable](https://img.shields.io/badge/23.05-Stable-green?style=flat-square)

| Architecture | Status |
|--------------|--------|
| `aarch64_cortex-a53` | ✅ Available |
| `aarch64_cortex-a72` | ✅ Available |
| `aarch64_cortex-a76` | ✅ Available |
| `aarch64_generic` | ✅ Available |
| `x86_64` | ✅ Available |

### ![Stable](https://img.shields.io/badge/24.10-Stable-green?style=flat-square)

| Architecture | Status |
|--------------|--------|
| `aarch64_cortex-a53` | ✅ Available |
| `aarch64_cortex-a72` | ✅ Available |
| `aarch64_cortex-a76` | ✅ Available |
| `aarch64_generic` | ✅ Available |
| `x86_64` | ✅ Available |

### ![SNAPSHOT](https://img.shields.io/badge/SNAPSHOT-Development-red?style=flat-square)

| Architecture | Status |
|--------------|--------|
| `aarch64_cortex-a53` | ✅ Available |
| `aarch64_cortex-a72` | ✅ Available |
| `aarch64_cortex-a76` | ✅ Available |
| `aarch64_generic` | ✅ Available |
| `x86_64` | ✅ Available |

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

Browse packages directly at: [📂 Package Browser](https://github.com/rizkikotet-dev/RTA-WRT_Packages/tree/releases)

### Method 3: Batch Installation Script

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

## 🛡️ Quality Assurance

- ✅ **Automated Testing**: All packages undergo validation
- 🔄 **Weekly Builds**: Fresh packages every week
- 📊 **Build Monitoring**: Failed builds are tracked and fixed
- 🏷️ **Version Tracking**: Clear versioning and changelog

## 🤝 Contributing

Want to add your packages? Here's how:

1. **Fork** this repository
2. **Add** your packages to the `packages/` directory and in .name-packages
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