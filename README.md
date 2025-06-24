# 🚀 OpenWRT Custom Packages Repository

## 📊 Repository Statistics

- **Total Packages**: 4456
- **Architectures**: 44
- **Branches**: 3
- **Repository Size**: 18MB

> Last updated: 2025-06-24 08:39:40 UTC

## 🌿 Supported OpenWRT Versions

### 23.05

| Architecture | Packages |
|--------------|----------|
| `aarch64_cortex-a53-openwrt` | 104 |
| `aarch64_cortex-a72-openwrt` | 104 |
| `aarch64_generic-openwrt` | 104 |
| `arm_cortex-a15_neon-vfpv4-openwrt` | 104 |
| `arm_cortex-a5_vfpv4-openwrt` | 104 |
| `arm_cortex-a7_neon-vfpv4-openwrt` | 104 |
| `arm_cortex-a8_vfpv3-openwrt` | 104 |
| `arm_cortex-a9-openwrt` | 104 |
| `arm_cortex-a9_neon-openwrt` | 104 |
| `arm_cortex-a9_vfpv3-d16-openwrt` | 104 |
| `i386_pentium4-openwrt` | 102 |
| `mips64_octeonplus-openwrt` | 102 |
| `mips_24kc-openwrt` | 102 |
| `mips_4kec-openwrt` | 69 |
| `mips_mips32-openwrt` | 102 |
| `mipsel_24kc_24kf-openwrt` | 102 |
| `mipsel_74kc-openwrt` | 102 |
| `mipsel_mips32-openwrt` | 102 |
| `x86_64-openwrt` | 102 |

### 24.10

| Architecture | Packages |
|--------------|----------|
| `aarch64_cortex-a53-openwrt` | 104 |
| `aarch64_cortex-a72-openwrt` | 104 |
| `aarch64_cortex-a76-openwrt` | 104 |
| `aarch64_generic-openwrt` | 104 |
| `arm_cortex-a15_neon-vfpv4-openwrt` | 104 |
| `arm_cortex-a5_vfpv4-openwrt` | 104 |
| `arm_cortex-a7_neon-vfpv4-openwrt` | 104 |
| `arm_cortex-a8_vfpv3-openwrt` | 104 |
| `arm_cortex-a9-openwrt` | 104 |
| `arm_cortex-a9_neon-openwrt` | 104 |
| `arm_cortex-a9_vfpv3-d16-openwrt` | 104 |
| `i386_pentium4-openwrt` | 102 |
| `mips64_octeonplus-openwrt` | 102 |
| `mips_24kc-openwrt` | 102 |
| `mips_4kec-openwrt` | 69 |
| `mips_mips32-openwrt` | 102 |
| `mipsel_24kc-openwrt` | 102 |
| `mipsel_24kc_24kf-openwrt` | 102 |
| `mipsel_74kc-openwrt` | 102 |
| `mipsel_mips32-openwrt` | 102 |
| `x86_64-openwrt` | 102 |

### SNAPSHOT

| Architecture | Packages |
|--------------|----------|
| `aarch64_cortex-a76` | 104 |
| `arm_cortex-a9_vfpv3-d16` | 92 |
| `mips_mips32` | 102 |
| `mipsel_24kc` | 102 |

## 🚀 Quick Start

```bash
# Add repository (replace [BRANCH] and [ARCH] with your values)
echo 'src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/[BRANCH]/[ARCH]' >> /etc/opkg/customfeeds.conf

# Update package lists
opkg update

# Install packages
opkg install [package_name]
```

Built with ❤️ using GitHub Actions
