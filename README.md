# 📦 OpenWRT Custom Packages Repository

This repository contains pre-built packages for various OpenWRT versions and architectures.

## 📊 Repository Statistics
- **Last updated**: 2025-06-22 13:17:41 UTC
- **Total packages**: 6187
- **Repository size**: 1134MB
- **Supported branches**: 3
- **Supported architectures**: 61

## 🏗️ Supported OpenWRT Versions

### 🔧 23.05
- **Packages**: 1925
- **Architectures**: 19

  - **aarch64_cortex-a53-openwrt**: 104 packages
  - **aarch64_cortex-a72-openwrt**: 104 packages
  - **aarch64_generic-openwrt**: 104 packages
  - **arm_cortex-a15_neon-vfpv4-openwrt**: 104 packages
  - **arm_cortex-a5_vfpv4-openwrt**: 104 packages
  - **arm_cortex-a7_neon-vfpv4-openwrt**: 104 packages
  - **arm_cortex-a8_vfpv3-openwrt**: 104 packages
  - **arm_cortex-a9-openwrt**: 104 packages
  - **arm_cortex-a9_neon-openwrt**: 104 packages
  - **arm_cortex-a9_vfpv3-d16-openwrt**: 104 packages
  - **i386_pentium4-openwrt**: 102 packages
  - **mips64_octeonplus-openwrt**: 102 packages
  - **mips_24kc-openwrt**: 102 packages
  - **mips_4kec-openwrt**: 69 packages
  - **mips_mips32-openwrt**: 102 packages
  - **mipsel_24kc_24kf-openwrt**: 102 packages
  - **mipsel_74kc-openwrt**: 102 packages
  - **mipsel_mips32-openwrt**: 102 packages
  - **x86_64-openwrt**: 102 packages

### 🔧 24.10
- **Packages**: 2131
- **Architectures**: 21

  - **aarch64_cortex-a53-openwrt**: 104 packages
  - **aarch64_cortex-a72-openwrt**: 104 packages
  - **aarch64_cortex-a76-openwrt**: 104 packages
  - **aarch64_generic-openwrt**: 104 packages
  - **arm_cortex-a15_neon-vfpv4-openwrt**: 104 packages
  - **arm_cortex-a5_vfpv4-openwrt**: 104 packages
  - **arm_cortex-a7_neon-vfpv4-openwrt**: 104 packages
  - **arm_cortex-a8_vfpv3-openwrt**: 104 packages
  - **arm_cortex-a9-openwrt**: 104 packages
  - **arm_cortex-a9_neon-openwrt**: 104 packages
  - **arm_cortex-a9_vfpv3-d16-openwrt**: 104 packages
  - **i386_pentium4-openwrt**: 102 packages
  - **mips64_octeonplus-openwrt**: 102 packages
  - **mips_24kc-openwrt**: 102 packages
  - **mips_4kec-openwrt**: 69 packages
  - **mips_mips32-openwrt**: 102 packages
  - **mipsel_24kc-openwrt**: 102 packages
  - **mipsel_24kc_24kf-openwrt**: 102 packages
  - **mipsel_74kc-openwrt**: 102 packages
  - **mipsel_mips32-openwrt**: 102 packages
  - **x86_64-openwrt**: 102 packages

### 🔧 SNAPSHOT
- **Packages**: 2131
- **Architectures**: 21

  - **aarch64_cortex-a53**: 104 packages
  - **aarch64_cortex-a72**: 104 packages
  - **aarch64_cortex-a76**: 104 packages
  - **aarch64_generic**: 104 packages
  - **arm_cortex-a15_neon-vfpv4**: 104 packages
  - **arm_cortex-a5_vfpv4**: 104 packages
  - **arm_cortex-a7_neon-vfpv4**: 104 packages
  - **arm_cortex-a8_vfpv3**: 104 packages
  - **arm_cortex-a9**: 104 packages
  - **arm_cortex-a9_neon**: 104 packages
  - **arm_cortex-a9_vfpv3-d16**: 104 packages
  - **i386_pentium4**: 102 packages
  - **mips64_octeonplus**: 102 packages
  - **mips_24kc**: 102 packages
  - **mips_4kec**: 69 packages
  - **mips_mips32**: 102 packages
  - **mipsel_24kc**: 102 packages
  - **mipsel_24kc_24kf**: 102 packages
  - **mipsel_74kc**: 102 packages
  - **mipsel_mips32**: 102 packages
  - **x86_64**: 102 packages


## 🚀 Usage

### Adding Repository to OpenWRT

```bash
# Add custom repository
echo "src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/[BRANCH]/[ARCH]" >> /etc/opkg/customfeeds.conf

# Update package lists
opkg update

# Install packages
opkg install [package_name]
```

### Direct Download

Browse and download packages directly from:
- 🌐 [GitHub Releases](https://github.com/rizkikotet-dev/RTA-WRT_Packages/tree/releases/packages)
- 📋 [Package Index](packages/repository.json)

## 🔄 Build Information

- **Source Repository**: [rizkikotet-dev/RTA-WRT_Packages](https://github.com/rizkikotet-dev/RTA-WRT_Packages)
- **Workflow Run**: [15806997807](https://github.com/rizkikotet-dev/RTA-WRT_Packages/actions/runs/15806997807)
- **Build Date**: 2025-06-22 13:17:42 UTC

---

*This repository is automatically updated via GitHub Actions*
