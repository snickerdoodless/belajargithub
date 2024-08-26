# Excercise 1: Managing Files & Folder Based on Their Extension
***

<br />

### Dilatihan ini kalian akan mencoba mengatur folder dan file berdasarkan ekstensi dengan linux command.

**Objective:**

Mengatur direktori yang berisi berbagai file dan subfolder dengan ekstensi berbeda ke dalam folder terpisah berdasarkan jenis file.

**Outcomes:**

Hasil latihan ini kalian akan bisa manage file dan folder berdasarkan ekstensi.

**1.**  Di multipass, `launch` atau buka `shell` instance kalian.
  <details>
    <summary>Lihat Solusi</summary>
    <code>multipass --launch lab-managing</code><br />
    <code>multipass shell lab-managing</code>
  </details>

<br />

**2**.  Pastikan kalian di `home`, buat 3 folder untuk file berbentuk `assets`, `source`  dan `etc` kemudian beri nama belakangnya `folder`.
  <details>
    <summary>Lihat Solusi</summary>
    <code>cd /home/ubuntu</code><br />
    <code>mkdir {assets,source,etc}-folder</code>
  </details>

<br />

**3**.  Buatlah 5 file `kosong` bernama source berekstensi `.js` dan 5 bernama front, 2 file bernama database dengan ekstensi `.db`, 1 dari ekstensi `.css` bernama style, 5 dari ekstensi `.jpg` bernama gambar, 3 dari `.gif` bernama gif, dan 3 dari `.mp3` bernama audio.
  <details>
    <summary>Lihat Solusi</summary>
    <code>touch {source,front}{1..5}.js ; touch database{1,2}.db</code><br />
    <code>touch style.css ; touch gambar{1..5}.jpg</code><br />
    <code>touch gif{1,2,3}.gif ; touch audio{1..3}.mp3</code>
  </details>

<br />

**4**.  Sekarang coba `konfirmasi` bahwa file kosong dan folder kosong sudah dibuat dan pastikan `tipe` nya
  <details>
    <summary>Lihat Solusi</summary>
    <code>ls -l</code><br />
    <code>file * > etc/type.txt</code><br />
    <code>cat etc/type.txt</code>
  </details>

<br />

**5**.  Kemudian buat folder baru dan buat ini sebagai `subfolder`, yang pertama dibawah assets buat folder bernama audio, image, dan gif folder, lakukan hal yang sama dengan source tetapi dengan nama frontend dan backend folder.
	<details>
	  <summary>Lihat Solusi</summary>
	    <code>mkdir -p assets/{audio, image, gif}</code><br />
	    <code>mkdir -p source/{frontend, backend}</code>
	</details>

<br />

**6**.  Pindahkan `semua` yang bernama source dan semua file bernama database ke folder `backend` dan pindahkan semua file yang bernama frontend ke folder `frontend`.
	<details>
	  <summary>Lihat Solusi</summary>
	    <code>mv source* database* source-folder/backend frontend* source-folder/frontend</code>
	</details>

<br />

**7**. Sama seperti tadi, sekarang pindahkan dan `sesuaikan` sisa file yang ada ke direktori masing-masing berdasarkan ekstensinya.
	<details>
	  <summary>Lihat Solusi</summary>
	    <code>mv gif* assets-folder/gif image* assets-folder/image audio* assets-folder/audio</code>
	</details>

<br />

**8**.  Konfirmasi bahwa semua file sudah tergoranisir berdasarkan folder tujuannya serta ekstensinya.
	<details>
	  <summary>Lihat Solusi</summary>
	    <code>ls assets-folder/gif assets-folder/image assets-folder/audio source-folder/frontend source-folder/backend > manage-structure.txt</code>
	</details>

