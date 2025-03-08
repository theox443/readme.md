# 1. Login ke server via SSH
ssh username@your-server-ip

# 2. Buat direktori proyek (jika belum ada)
mkdir -p ~/projects/gitigrone-theox443
cd ~/projects/gitigrone-theox443

# 3. Buat file README.md dengan konten dasar
cat > README.md <<EOF
# Gitigrone Theox443

![Project Banner](assets/banner.png) <!-- Opsional -->

Proyek untuk mengelola konfigurasi dan automasi sistem Theox443.

## Fitur Utama
- [ ] Manajemen konfigurasi sistem
- [ ] Automasi deployment
- [ ] Monitoring resources
- [ ] Integrasi CI/CD

## Prasyarat
- Bash 4.0+
- SSH client
- Python 3.8+ (opsional)
- Docker (opsional)

## Instalasi
\`\`\`bash
# Clone repositori
git clone ssh://git@your-server:port/gitigrone-theox443.git
cd gitigrone-theox443

# Berikan hak akses eksekusi
chmod +x setup.sh

# Jalukan setup
./setup.sh
\`\`\`

## Konfigurasi
Salin file contoh konfigurasi:
\`\`\`bash
cp config.example.yaml config.yaml
\`\`\`

Edit file config.yaml sesuai kebutuhan sistem Anda.

## Penggunaan
\`\`\`bash
# Mode interaktif
./gitigrone.sh --interactive

# Mode daemon
./gitigrone.sh --daemon
\`\`\`

## Struktur Direktori
\`\`\`
.
├── src/           # Kode sumber utama
├── config/        # File konfigurasi
├── docs/          # Dokumentasi
├── scripts/       # Skrip utilitas
└── tests/         # Test cases
\`\`\`

## Kontribusi
1. Fork repositori
2. Buat branch fitur (\`git checkout -b fitur/namafitur\`)
3. Commit perubahan (\`git commit -am 'Tambahkan fitur'\`)
4. Push ke branch (\`git push origin fitur/namafitur\`)
5. Buat Pull Request

## Lisensi
MIT © 2024 Pemilik Proyek
EOF

# 4. Verifikasi file
cat README.md
