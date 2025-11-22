# Panduan Lengkap Perintah File dan Direktori di Terminal

## 🧭 Navigasi (Navigation)

| Perintah | Fungsi |
|----------|--------|
| `pwd` | Menampilkan lokasi folder saat ini |
| `ls` | Menampilkan daftar isi folder |
| `ls -la` | Menampilkan semua file (termasuk tersembunyi) secara detail |
| `ls -R` | Menampilkan semua isi folder dan subfoldernya |
| `cd nama-folder` | Masuk ke folder tertentu |
| `cd ..` | Kembali ke folder sebelumnya (naik 1 level) |
| `cd ../..` | Kembali 2 level ke atas |
| `cd folder1/folder2` | Masuk ke folder bertingkat sekaligus |
| `clear` | Membersihkan layar terminal |

## 🛠️ Manipulasi (Manipulation)

### 📁 Membuat File dan Folder

| Perintah | Fungsi |
|----------|--------|
| `mkdir nama-folder` | Membuat folder baru di lokasi saat ini |
| `mkdir -p folder1/folder2/folder3` | Membuat folder bertingkat sekaligus |
| `touch nama-file.txt` | Membuat file baru (kosong) |

### ✏️ Menulis ke File

| Perintah | Fungsi |
|----------|--------|
| `echo "teks" > file` | Menulis teks ke file (menimpa isi lama) |
| `echo "teks" >> file` | Menambah teks ke akhir file (tidak menimpa) |
| `cat file-a > file-b` | Salin isi file-a ke file-b (menimpa isi file-b) |
| `cat file-a >> file-b` | Tambahkan isi file-a ke akhir file-b |

### 🔄 Memindahkan dan Mengganti Nama

| Perintah | Fungsi |
|----------|--------|
| `mv file-lama file-baru` | Mengganti nama file |
| `mv file target-folder/` | Memindahkan file ke folder lain |
| `mv folder-lama folder-baru` | Mengganti nama folder |
| `mv folder target-folder/` | Memindahkan folder ke folder lain |

### 🗑️ Menghapus File dan Folder

| Perintah | Fungsi |
|----------|--------|
| `rm file` | Menghapus file |
| `rm -r folder` | Menghapus folder beserta isinya |
| `rmdir folder` | Menghapus folder kosong |
| `rm -rf folder` | Menghapus folder paksa (hati-hati!) |
| `rm *.txt` | Menghapus semua file dengan ekstensi .txt |

### 📋 Menyalin File dan Folder

| Perintah | Fungsi |
|----------|--------|
| `cp file-a file-b` | Salin file-a menjadi file-b (menimpa jika ada) |
| `cp file folder/` | Salin file ke dalam folder |
| `cp -r folder-a folder-b` | Salin folder beserta isinya |
| `cp *.txt folder/` | Salin semua file .txt ke folder |

## 📖 Membaca File

| Perintah | Fungsi |
|----------|--------|
| `cat file` | Tampilkan seluruh isi file |
| `echo "output-here"` | Menampilkan teks yang diketik |
| `head file` | Tampilkan 10 baris pertama |
| `tail file` | Tampilkan 10 baris terakhir |
| `less file` | Baca file dengan scroll (tekan q untuk keluar) |

## 🔍 Mencari File

| Perintah | Fungsi |
|----------|--------|
| `find . -name "*.txt"` | Cari semua file .txt di folder ini |
| `grep "kata" file` | Cari kata tertentu dalam file |

## ⚙️ Operator (Operators)

| Operator | Fungsi | Contoh |
|----------|--------|--------|
| `>` | Menimpa isi file dengan hasil perintah | `echo "Hello, World" > file.txt` |
| `>>` | Menambah hasil perintah ke akhir file | `echo "Hello, World" >> file.txt` |
| `;` | Menjalankan beberapa perintah berurutan | `echo "Howdy there!" ; cat file.txt` |
| `\|\|` | Menjalankan perintah alternatif jika perintah pertama gagal | `mkdir work \|\| echo "Directory creation failed. Does it already exist?"` |
| `&&` | Menjalankan perintah kedua hanya jika perintah pertama berhasil | `mkdir video-games && cd video-games` |

## ⌨️ Shortcut Keyboard

| Shortcut | Fungsi |
|----------|--------|
| `Tab` | Melengkapi nama file atau folder secara otomatis |
| `↑` / `↓` | Mengulangi perintah yang sudah diketik sebelumnya |
| `Ctrl + L` atau `Command + K` | Membersihkan layar terminal |
| `Ctrl + C` | Membatalkan perintah yang sedang berjalan |

---

## ⚠️ Peringatan Penting

- **Simbol `>` menimpa isi file**, gunakan `>>` untuk menambah
- **`rm -rf` sangat berbahaya** - file yang terhapus tidak bisa dikembalikan!
- **Gunakan `-r` untuk folder** - cp dan rm memerlukan flag ini untuk folder
- **Cek dulu dengan `ls`** sebelum menghapus atau memindahkan file

## 💡 Tips Tambahan

- Gunakan **Tab** untuk autocomplete nama file/folder
- Gunakan **tanda kutip** jika nama file ada spasi: `"nama file.txt"`
- Gunakan **`./`** untuk merujuk folder saat ini
- Gunakan **`../`** untuk merujuk folder di atasnya
- Gunakan **`~`** untuk merujuk folder home 
