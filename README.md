# PROJECT-SO-ANDRI5.1

### Langkah 1: Persiapan - Buat Folder Utama
Folder utama bernama "MyFiles" akan dibuat di direktori home Anda (`~/MyFiles`).

1. Buka Terminal.
2. Jalankan perintah berikut untuk membuat folder utama:
   ```
   mkdir ~/MyFiles
   ```
   - Ini membuat folder `MyFiles` di `/home/your_username/MyFiles` (ganti `your_username` dengan nama pengguna Anda).

### Langkah 2: Struktur Folder - Buat Subfolder dengan Minimal 5 Kategori
Kita akan buat subfolder di dalam `MyFiles`. Untuk tugas ini, saya pilih **5 kategori berbeda** yang cocok untuk file kuliah/pekerjaan semester 1:
- **Lectures**: Untuk catatan kuliah atau slide presentasi.
- **Assignments**: Untuk tugas-tugas harian atau mingguan.
- **Projects**: Untuk proyek kelompok atau individu.
- **Resources**: Untuk bahan referensi seperti buku, artikel, atau link.
- **Exams**: Untuk soal ujian, kuis, atau bahan persiapan ujian.

Jalankan perintah berikut untuk membuat semua subfolder sekaligus:
```
mkdir ~/MyFiles/Lectures ~/MyFiles/Assignments ~/MyFiles/Projects ~/MyFiles/Resources ~/MyFiles/Exams
```
- Ini membuat 5 subfolder di dalam `MyFiles`.

### Langkah 3: Organisasi - Pindahkan File ke Folder yang Sesuai
Gunakan perintah `mv` (move) untuk memindahkan file. Jika belum ada file, buat file dummy terlebih dahulu dengan `touch` (misalnya, untuk simulasi).

Contoh simulasi:
- Buat file dummy di `MyFiles`:
  ```
  touch ~/MyFiles/lecture_notes.txt ~/MyFiles/assignment1.pdf ~/MyFiles/project_code.py ~/MyFiles/resource_book.pdf ~/MyFiles/exam_prep.docx
  ```
- Pindahkan file ke kategori yang sesuai:
  ```
  mv ~/MyFiles/lecture_notes.txt ~/MyFiles/Lectures/
  mv ~/MyFiles/assignment1.pdf ~/MyFiles/Assignments/
  mv ~/MyFiles/project_code.py ~/MyFiles/Projects/
  mv ~/MyFiles/resource_book.pdf ~/MyFiles/Resources/
  mv ~/MyFiles/exam_prep.docx ~/MyFiles/Exams/
  ```
- Jika Anda punya file asli (misalnya, dari Downloads), ganti nama file di atas dengan nama file Anda. Contoh: `mv ~/Downloads/my_lecture.pdf ~/MyFiles/Lectures/`.

### Langkah 4: Verifikasi - Lihat Struktur Folder
Gunakan perintah `tree` untuk melihat struktur folder yang telah dibuat. Jika `tree` belum terinstall, install dulu dengan `sudo apt install tree`.

Jalankan:
```
tree ~/MyFiles
```
- Outputnya akan terlihat seperti ini (contoh setelah memindahkan file):
  ```
  /home/your_username/MyFiles
  ├── Assignments
  │   └── assignment1.pdf
  ├── Exams
  │   └── exam_prep.docx
  ├── Lectures
  │   └── lecture_notes.txt
  ├── Projects
  │   └── project_code.py
  └── Resources
      └── resource_book.pdf
  ```
- Ini menunjukkan struktur folder dengan 5 kategori dan file yang telah dipindahkan.

### Tips Tambahan untuk Semester 1:
- **Kustomisasi**: Jika mata kuliah Anda berbeda (misalnya, tambah "Labs" untuk praktikum), buat subfolder tambahan dengan `mkdir ~/MyFiles/Labs`.
- **Backup**: Untuk keamanan, salin folder ini ke cloud (misalnya, Google Drive) dengan `cp -r ~/MyFiles /path/to/cloud/folder`.
- **Otomatisasi**: Jika sering melakukan ini, buat script Bash sederhana. Buat file `organize.sh` dengan isi:
  ```
  #!/bin/bash
  mkdir -p ~/MyFiles/{Lectures,Assignments,Projects,Resources,Exams}
  echo "Folders created!"
  ```
  - Jalankan dengan `chmod +x organize.sh && ./organize.sh`.
- **Troubleshooting**: Jika ada error izin, gunakan `sudo` untuk perintah mkdir/mv, tapi hindari di home directory.

Jika Anda mengikuti langkah ini, sistem foldersudah siap.
