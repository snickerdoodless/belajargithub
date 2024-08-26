
# Excercise 1: Managing Files & Folder Based on Their Extension
***

<br />

## Dilatihan ini kalian akan mencoba mengatur folder dan file berdasarkan ekstensi dengan linux command.

**Objective:**

Mengatur direktori yang berisi berbagai file dan subfolder dengan ekstensi berbeda ke dalam folder terpisah berdasarkan jenis file.

**Outcomes:**

Hasil latihan ini kalian akan bisa manage file dan folder berdasarkan ekstensi.

**1.**  Di multipass, `launch` atau buka `shell` instance kalian.
 
<details>
  <summary>Lihat Solusi</summary>
  <code>ls -l<br>file * > etc/type.txt</code> 
  <code>cat etc/type.txt</code>
</details>

<br />

2.  Pastikan kalian di `home`, buat 3 folder untuk file berbentuk `assets`, `source`  dan `etc` kemudian beri nama belakangnya `folder`.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    cd /home/ubuntu<br>
	    mkdir {assets,source,etc}-folder
	  </p>
	</details>

<br />

3.  Buatlah 5 file `kosong` bernama source berekstensi `.js` dan 5 bernama front, 2 file bernama database dengan ekstensi `.db`, 1 dari ekstensi `.css` bernama style, 5 dari ekstensi `.jpg` bernama gambar, 3 dari `.gif` bernama gif, dan 3 dari `.mp3` bernama audio.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    touch {source,front}{1..5}.js ; touch database{1,2}.db<br>
	    touch style.css ; touch gambar{1..5}.jpg<br>
	    touch gif{1,2,3}.gif ; touch audio{1..3}.mp3
	  </p>
	</details>

<br />

4.  Sekarang coba `konfirmasi` bahwa file kosong dan folder kosong sudah dibuat dan pastikan `tipe` nya.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    ls -l<br>
	    file * > etc/type.txt<br>
	    cat etc/type.txt
	  </p>
	</details>

5.  Kemudian buat folder baru dan buat ini sebagai `subfolder`, yang pertama dibawah assets buat folder bernama audio, image, dan gif folder, lakukan hal yang sama dengan source tetapi dengan nama frontend dan backend folder.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    mkdir -p assets/{audio, image, gif}<br>
	    mkdir -p source/{frontend, backend}
	  </p>
	</details>
