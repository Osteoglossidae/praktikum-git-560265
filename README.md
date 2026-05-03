# praktikum-git-560265

> Repositori untuk Praktikum Git & GitHub — Pemrograman Web 2025/2026

---
## Langkah Pengerjaan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/Osteoglossidae/praktikum-git-560265.git
   cd praktikum-git-560265
   ```

2. Buat index.html, style.css dan .gitignore menggunakan command yang sama
   ```bash
   #sebelumnya pastikan lokasi direktori benar
   touch namafile.extension
   ```
---

## 🌐 Tampilan Website

<img width="1905" height="938" alt="image" src="https://github.com/user-attachments/assets/6f654470-e367-4ed6-a28b-e598b9c16d26" />

---

## 🌿 Git Log

<img width="747" height="209" alt="Screenshot 2026-05-02 181235" src="https://github.com/user-attachments/assets/998b61f1-76f2-43cf-b357-86e41ad64bd3" />

---

## 📸 Branch Protection Rule

> *(Letakkan screenshot Branch Protection Rule settings di sini)*

![Branch Protection](screenshot-branch-protection.png)

---

## Command Git yang Digunakan

### Inisialisasi & Commit Dasar

```bash
# Inisialisasi atau clone repository
git clone <url>
cd <nama-repo>

# Cek status file
git status

# Tambahkan file ke staging area
git add <nama-file>
git add .              # tambah semua file

# Buat commit
git commit -m "pesan commit"

# Kirim ke remote
git push origin main

# Lihat riwayat commit
git log --oneline --graph
```

### Branching

```bash
# Buat dan pindah ke branch baru
git checkout -b nama-branch

# Pindah ke branch yang sudah ada
git checkout nama-branch

# Lihat semua branch
git branch -a

# Hapus branch lokal
git branch -d nama-branch

# Hapus branch remote
git push origin --delete nama-branch
```

### Merge & Konflik

```bash
# Merge branch lain ke branch aktif
git merge nama-branch

# Setelah selesaikan konflik manual:
git add file-yang-konflik
git commit -m "fix: resolve merge conflict"
```

Penyelesaian konflik menggunakan VScode:
<img width="1124" height="762" alt="Screenshot 2026-05-03 070416" src="https://github.com/user-attachments/assets/a0ef201b-855d-4a71-9428-e4740df8368d" />


### Interactive Rebase

```bash
# Squash 3 commit terakhir menjadi 1
git rebase -i HEAD~3

# Di editor yang muncul:
# pick  abc123 commit pertama     → biarkan 'pick'
# squash def456 commit kedua      → ubah jadi 'squash'
# squash ghi789 commit ketiga     → ubah jadi 'squash'
# Simpan, lalu tulis pesan commit baru
```

### Pull Request

```bash
# Push branch ke remote sebelum buat PR
git push origin nama-branch

# Buka GitHub → Pull requests → New pull request
# Pilih base: main  ←  compare: nama-branch
```

---
