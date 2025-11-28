 
#### Langkah 1: Persiapan - Buat Folder Utama
Buat folder utama bernama "KuliahFiles" di drive D:.

```
mkdir D:\KuliahFiles
```

#### Langkah 2: Struktur Folder - Buat Subfolder dengan Minimal 5 Kategori
Saya sarankan 5 kategori berbeda untuk file kuliah, misalnya:
- **Lectures**: Untuk file rekaman atau slide kuliah.
- **Assignments**: Untuk tugas-tugas yang diberikan.
- **Notes**: Untuk catatan pribadi atau ringkasan.
- **Projects**: Untuk proyek kelompok atau individu.
- **Resources**: Untuk bahan tambahan seperti artikel, buku, atau referensi.

Gunakan perintah `mkdir` untuk membuat subfolder ini di dalam "KuliahFiles":

```
mkdir D:\KuliahFiles\Lectures
mkdir D:\KuliahFiles\Assignments
mkdir D:\KuliahFiles\Notes
mkdir D:\KuliahFiles\Projects
mkdir D:\KuliahFiles\Resources
```

#### Langkah 3: Organisasi - Pindahkan File ke Folder yang Sesuai
Jika Anda sudah memiliki file kuliah di lokasi lain (misalnya di Desktop atau folder sementara), gunakan perintah `move` untuk memindahkannya. Contoh:
- Misalkan ada file "lecture1.pdf" di D:\Temp, pindahkan ke Lectures:
  ```
  move D:\Temp\lecture1.pdf D:\KuliahFiles\Lectures\
  ```
- Lakukan hal serupa untuk file lainnya sesuai kategori. Jika belum ada file, Anda bisa menambahkannya nanti.

#### Langkah 4: Verifikasi - Lihat Struktur Folder
Gunakan perintah `tree` untuk melihat struktur folder yang telah dibuat:

```
tree D:\KuliahFiles /F
```

Ini akan menampilkan output seperti:
```
D:\KULIAHFILES
├── Lectures
├── Assignments
├── Notes
├── Projects
└── Resources
```

#### Tips Tambahan
- **Kustomisasi**: Jika Anda ingin lebih dari 5 kategori (misalnya tambahkan "Exams" untuk ujian), cukup buat subfolder baru dengan `mkdir`.
- **Otomatisasi**: Untuk efisiensi, Anda bisa membuat script batch (.bat) yang menjalankan semua perintah di atas sekaligus.
- **Keamanan**: Pastikan folder ini di-backup secara berkala, misalnya ke cloud storage seperti Google Drive atau OneDrive.
- **Alternatif GUI**: Jika lebih suka antarmuka grafis, buat folder melalui File Explorer Windows.
