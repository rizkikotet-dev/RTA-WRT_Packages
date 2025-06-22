# 📦 OpenWRT Custom Packages Repository

![Build Status](https://github.com/rizkikotet-dev/RTA-WRT_Packages/actions/workflows/build.yaml/badge.svg)
![License](https://img.shields.io/github/license/rizkikotet-dev/RTA-WRT_Packages)
![GitHub Repo Size](https://img.shields.io/github/repo-size/rizkikotet-dev/RTA-WRT_Packages)

Welcome to the **OpenWRT Custom Packages Repository**! This repository provides pre-built custom packages for various OpenWRT versions and architectures, making it easy to extend your OpenWRT firmware with additional functionality.

## 🚀 Features

- Supports multiple architectures: aarch64 (cortex-a53, cortex-a72, cortex-a76, generic), x86_64
- Compatible with OpenWRT branches: openwrt-23.05, openwrt-24.10, SNAPSHOT
- Automated build and release with GitHub Actions
- Repository size management for optimal storage
- Comprehensive metadata generation for package indexing

## 📦 Usage

### ➕ Adding the Repository to OpenWRT

Add the custom package feed to your OpenWRT device by appending the following line to `/etc/opkg/customfeeds.conf`:

```bash
echo "src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/[BRANCH]/[ARCH]" >> /etc/opkg/customfeeds.conf
opkg update
```

Replace `[BRANCH]` and `[ARCH]` with your OpenWRT branch and device architecture respectively.

### 📥 Installing Packages

After updating the feeds, install packages using:

```bash
opkg install [package_name]
```

### 🌐 Direct Download

Browse and download packages directly from:

- [GitHub Releases](https://github.com/rizkikotet-dev/RTA-WRT_Packages/tree/releases/packages)
- [Package Index](packages/repository.json)

## 🏗️ Build and Release Workflow

This project leverages GitHub Actions to automate building, packaging, and releasing OpenWRT packages for multiple architectures and branches. The workflow includes:

- ✅ Checkout and setup build environment
- 🛠️ Build packages using OpenWRT SDK
- 📂 Organize packages into structured directories
- 📄 Generate package manifests and metadata
- 🧹 Manage repository size and clean up old packages
- 🚀 Commit and push release artifacts to the `releases` branch

## 📊 Repository Statistics

The repository is regularly updated with new packages and metadata to ensure users have access to the latest builds.

---

*This repository is automatically maintained via GitHub Actions workflows.*
