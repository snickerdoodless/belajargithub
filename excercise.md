
# Excercise 1: Managing Files & Folder Based on Their Extension
***

Dilatihan ini kalian akan mencoba mengatur folder dan file berdasarkan ekstensi dengan linux command.

**Outcomes**

Hasil latihan ini kalian akan bisa manage file dan folder berdasarkan ekstensi.

1.  Di multipass, `launch` atau buka `shell` instance kalian.
 
html
<style>
  details {
    background-color: #f0f0f0; /* add a light gray background to the details element */
  }

  details p {
    color: #00698f; /* set the text color to a blue-ish hue */
  }
</style>

<details>
  <summary>Lihat Solusi<br>Klik untuk melihat jawaban</summary>
  <p>
    multipass launch --name ubuntu<br>
    multipass shell ubuntu
  </p>
</details>

2.  Pastikan kalian di `home`, buat 3 folder untuk file berbentuk `assets`, `source`  dan `etc` kemudian beri nama belakangnya `folder`.

	<details>
	  <summary>Lihat Solusi</summary>
	  <p>
	    pwd<br> # /home/ubuntu
	    mkdir {assets,source,etc}-folder
	  </p>
	</details>
