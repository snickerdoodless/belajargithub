# Excercise 1: Managing Files & Folder Based on Their Extension
***

<br />

##### Dilatihan ini kalian akan mencoba mengatur folder dan file berdasarkan ekstensi dengan linux command.

**Objective:**

Mengatur direktori yang berisi berbagai file dan subfolder dengan ekstensi berbeda ke dalam folder terpisah berdasarkan jenis file.

**Outcomes:**

Hasil latihan ini kalian akan bisa manage file dan folder berdasarkan ekstensi.

1.  Di multipass, `launch` atau buka `shell` instance kalian.
 
	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    multipass launch --name ubuntu<br>
	    multipass shell ubuntu
	  </p>
	</details>

<br />

2.  Pastikan kalian di `home`, buat 3 folder untuk file berbentuk `assets`, `source`  dan `etc` kemudian beri nama belakangnya `folder`.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    cd /home/ubuntu
	    mkdir {assets,source,etc}-folder
	  </p>
	</details>

<br />

3.  Buatlah 10 file `kosong` bernama source berekstensi `.js`, 2 file bernama database dengan ekstensi `.db`, 1 dari ekstensi `.css` bernama style, 5 dari ekstensi `.jpg` bernama gambar, 3 dari `.gif` bernama gif, dan 3 dari `.mp3` bernama audio.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    touch source{1..10}.js ; touch database{1,2}.db<br>
	    touch style.css ; touch gambar{1..5}.jpg<br>
	    touch gif{1,2,3}.gif ; touch audio{1..3}.mp3
	  </p>
	</details>
	
