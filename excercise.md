
# Excercise 1: Creating and Managing Files and Folder Based on Their Extension
***

#### Dalam latihan ini, Kalian akan mengatur folder dan file berdasarkan ekstensinya menggunakan perintah Linux.

**Objective:**

Mempelajari cara mengelola dan mengimplementasikan struktur direktori dengan mengelompokkan file dan subfolder berdasarkan ekstensi ke dalam folder terpisah sesuai jenis file.

**Outcomes:**

Peserta akan mampu mengelola file dan folder berdasarkan ekstensi, termasuk memindahkan dan mengatur file secara efisien ke dalam direktori yang sesuai menggunakan perintah Linux.

<br />

**1.**  Di Multipass, buat instance dengan `launch` atau buka `shell` instance yang sudah ada.
***
**2**.  Pastikan kalian di `home` dan clone repository berikut
***
```
https://github.com/Komandro-CCIT/devops-exercise.git
```

**3**. Masuk ke folder `exercise-1` fokuskan untuk selesaikan exercise ini terlebih dahulu sebelum yang ke-2

**4**. Kemudian buat folder baru bernama `static`, `media` dan `code`.

Expected Output:
![](assets/latihan/exercise-1.1.png)

**6**.  Pindahkan `semua` file yang berekstensikan `.js` dan `.css` kedalam folder `code`.

**7**. Sama seperti tadi, sekarang pindahkan dan semua file yang berekstensikan `.png` kedalam folder `static`.

**8**. Terakhir pindahkan sisa file yang ada ke dalam folder `media`.

**9**. List semua folder agar terlihat secara terstruktur dan terorganisir berdasarkan ekstensinya.

Expected Output:

![](assets/latihan/exercise-1.2.png)

Selamat kalian sudah bisa menguasai bagaimana caranya mengatur file dan folder berdasarkan ekstensi 🥳.

<br />

## **Reason Why You Should Organize Your File Based On Extension:**

- **Easier Navigation and Location**
	Lebih mudah untuk navigasi direktori project dan mencari file tertentu. Misalnya, kalau kalian perlu cari file JavaScript, mereka hanya mencarinya di folder code, js, source atau javascript folder.
- **Better Collaboration**
	Anggota tim dapat dengan cepat dan paham struktur project dan mencari file yang mereka butuhkan untuk bekerja. Ini mengurangi kebingungan dan misskomunikasi.
- **Enhanced Security**
	Organize file berdasarkan ekstensi juga dapat meningkatkan keamanan. Contohnya memisahkan file sensitif, file konfigurasi atau encryption key ke dalam folder khusus mereka, developer dapat lebih mudah kontrol akses dan mengurangi resiko unauthorized access.
- **Simplified Build and Deployment**
	Banyak tools build and deployment scripts bergantung pada file extensionya untuk menentukan proses packaging files. Organizing files by extension lebih mudah untuk konfigurasikan toolsnya dan memastikan files lancar pada saat proses build and deployment.
- **Reduced Errors and Conflicts**
	Organizing files by extension meminimalisirkan resiko error dan konflik antar files, Contohnya ketika files tidak terorganize anggota tim terkadang tidak sengaja mengubah file yang salah membuat project error tidak karuan dan sulit untuk di identifikasi.

<br />

# Excercise 2: Creating Backup Files with Timestamp Along With Source and Destination Folder
***

#### Dalam latihan ini, Kalian akan mencoba membuat file menggunakan stempel waktu, serta menentukan folder source dan destination menggunakan perintah Linux.

**Objective:**

Memahami dan mempraktikkan pembuatan file cadangan dengan stempel waktu menggunakan perintah Linux, serta mengatur folder sumber (source) dan tujuan (destination) untuk menyimpan file tersebut.

**Outcomes:**

Peserta akan dapat membuat file cadangan dengan stempel waktu yang unik, menentukan dan menggunakan direktori sumber dan tujuan yang berbeda, serta mengembangkan pemahaman yang lebih baik tentang manajemen file dan direktori di lingkungan Linux.

**1.**  Di Multipass, buka `shell` instance kalian, lalu pastikan kalian berada di direktori `home`.

**2.** Melanjutkan `exercise-1` sekarang `exercise-2` akan menggunakan file yang berada di `exercise-1` untuk sebagai source foldernya.

**3.** Masuk ke folder `exercise-1` untuk memulai latihan yang ke-2.

**4.** Buat variabel global bernama `TIMESTAMP` di commandline interface, beri valuenya dengan command `date` dan spesifikan waktunya berdasarkan `YYYY-MM-DD_hh:mm:ss` gunakan man untuk melihat formatnya lalu pastikan variabelnya terbuat.  

Expected Output:
![](assets/latihan/exercise-2.1.png)

**5.** Sekarang backup folder `code` yang ada didalam `exercise-1` dengan folder `exercise-2/target-a` sebagai destination dan beri ekstensi `tar.gz` menggunakan perintah `tar` linux, gunakan `man` untuk caranya, dan untuk nama file backup tersebut yaitu variabel `TIMESTAMP` yang baru dibuat.

Expected Output:

![](assets/latihan/exercise-2.2.png)

**6.** Lakukan hal yang sama untuk folder `media` dan `static` ke folder `exercise-2/target-b` dan `exercise-2/target-c`, tapi sebelum backup menggunakan `tar` jalankan command membuat variable global `TIMESTAMP` secara bergantian dengan `media` kemudian backup dan `static` dan backup juga, ini dilakukan agar waktu di variabelnya terupdate, kemudian tampilkan semua backup secara terstruktur.

Expected Output:

![](assets/latihan/exercise-2.3.png)

**7.** Sekarang hapus semua file yang ada di `target-a`, `target-b`, `target-c`.

Expected Output:

![](assets/latihan/exercise-2.4.png)

**8.** Pindah 1 direktori ke belakang dan buatlah `bash script` bernama `backup.sh` dengan command-command yang kalian sudah gunakan untuk backup file dari `step-step sebelumnya`.

**9.** Berikan `execute permission` pada scriptnya dan jalankan scriptnya.

**10.** List lagi hasil backup yang menggunakan script

Expected Output:

![](assets/latihan/exercise-2.5.png)

Selamat kalian sudah bisa menguasai bagaimana caranya backup file dan folder dengan `tar` command di linux 🥳.

<br />

## **Reason Why You Should Backup Your File & Folder Frequently:**

- **Data Loss Prevention**
	Untuk alasan ini sudah pasti sangat wajib dan mutlak, agar kejadian seperti yang dialami kementrian teknologi dan komunikasi itu tidak terjadi pada kalian.
- **Version Control and Rollback**
	Terkadang update yang dilakukan pada suatu project itu tidak sesuai ekspektasi, dengan adanya backup kita bisa rollback ke versi sebelumnya.
- **Knowledge Archiving**
	File & Folder backup saat sudah tidak bisa dipakai bisa menjadi archive untuk kebutuhan masa mendatang

<br />
