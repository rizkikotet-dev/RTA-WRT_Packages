# 📦 Repositori Paket Kustom OpenWRT

![Status Build](https://github.com/rizkikotet-dev/RTA-WRT_Packages/actions/workflows/build.yaml/badge.svg)
![Lisensi](https://img.shields.io/github/license/rizkikotet-dev/RTA-WRT_Packages)
![Ukuran Repo GitHub](https://img.shields.io/github/repo-size/rizkikotet-dev/RTA-WRT_Packages)

Selamat datang di **Repositori Paket Kustom OpenWRT**! Repositori ini menyediakan paket kustom yang sudah dibangun untuk berbagai versi dan arsitektur OpenWRT, memudahkan Anda untuk memperluas firmware OpenWRT dengan fungsionalitas tambahan.

## 🚀 Fitur

- Mendukung berbagai arsitektur: aarch64 (cortex-a53, cortex-a72, cortex-a76, generic), x86_64
- Kompatibel dengan cabang OpenWRT: openwrt-23.05, openwrt-24.10, SNAPSHOT
- Build dan rilis otomatis menggunakan GitHub Actions
- Manajemen ukuran repositori untuk penyimpanan optimal
- Pembuatan metadata lengkap untuk pengindeksan paket

## 📦 Penggunaan

### ➕ Menambahkan Repositori ke OpenWRT

Tambahkan feed paket kustom ke perangkat OpenWRT Anda dengan menambahkan baris berikut ke `/etc/opkg/customfeeds.conf`:

```bash
echo "src/gz custom_packages https://raw.githubusercontent.com/rizkikotet-dev/RTA-WRT_Packages/releases/packages/[BRANCH]/[ARCH]" >> /etc/opkg/customfeeds.conf
opkg update
```

Ganti `[BRANCH]` dan `[ARCH]` dengan cabang OpenWRT dan arsitektur perangkat Anda masing-masing.

### 📥 Menginstal Paket

Setelah memperbarui feed, instal paket menggunakan:

```bash
opkg install [nama_paket]
```

### 🌐 Unduh Langsung

Telusuri dan unduh paket langsung dari:

- [GitHub Releases](https://github.com/rizkikotet-dev/RTA-WRT_Packages/tree/releases/packages)
- [Indeks Paket](packages/repository.json)

## 🏗️ Proses Build dan Rilis

Proyek ini memanfaatkan GitHub Actions untuk mengotomatisasi build, pengemasan, dan rilis paket OpenWRT untuk berbagai arsitektur dan cabang. Proses ini meliputi:

- ✅ Checkout dan setup lingkungan build
- 🛠️ Membangun paket menggunakan OpenWRT SDK
- 📂 Mengorganisir paket ke dalam direktori terstruktur
- 📄 Membuat manifest dan metadata paket
- 🧹 Mengelola ukuran repositori dan membersihkan paket lama
- 🚀 Commit dan push artefak rilis ke cabang `releases`

## 📊 Statistik Repositori

Repositori ini secara rutin diperbarui dengan paket dan metadata terbaru untuk memastikan pengguna mendapatkan build terbaru.

---

*Repositori ini secara otomatis dikelola melalui workflow GitHub Actions.*
