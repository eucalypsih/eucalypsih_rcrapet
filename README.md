# eucalypsih_rcrapet

Mematikan Fitur History Secara Permanen
Jika Anda tidak ingin Micro merekam atau mengingat riwayat pencarian dan perintah Anda lagi di masa mendatang:
```
setg savehistory false
```

```
rm -f ~/.config/micro/buffers/history
```

Jika Menggunakan Struktur Folder XDG Modern:
```
rm -f ~/.local/state/micro/buffers/history
```

Menghapus Total History Micro
Pastikan Anda sudah keluar dari editor Micro (Ctrl + Q), lalu jalankan perintah pembersihan ini di terminal Termux Anda:


Di editor Micro, kata kunci `find` digunakan untuk mencari teks di dalam file yang sedang Anda buka. Fungsi ini bertindak sebagai fitur pencarian standar (*Search/Find*).

Berikut adalah cara menggunakan fitur pencarian dan navigasinya di Micro:

1. Cara Mencari Teks (`Ctrl + F`)
- Tekan kombinasi tombol `Ctrl + F`.
- Baris perintah di bagian bawah layar akan memunculkan perintah `find: `.
- Ketik kata atau kode yang ingin Anda cari, lalu tekan `Enter`.
- Micro akan langsung melompat dan menyorot kata pertama yang cocok.

2. Navigasi Hasil Pencarian
Setelah Anda menekan Enter dan teks ditemukan, gunakan pintasan ini untuk berpindah antar hasil:
- Ke hasil berikutnya (Maju): Tekan Ctrl + N (Next).
- Ke hasil sebelumnya (Mundur): Tekan Ctrl + P (Previous).


Alternative: Menggunakan Perintah Ctrl + E
Selain menggunakan pintasan Ctrl + F, Anda juga bisa mengetikkan perintah pencarian secara manual melalui baris perintah:
- Tekan Ctrl + E.
- Ketik find <kata_yang_dicari> (misal: find fun).
- Tekan Enter.


Fitur Pencarian Tingkat Lanjut (Regex)
Micro juga mendukung pencarian menggunakan pola karakter atau Regular Expression (Regex).
- Contoh: Jika Anda ingin mencari semua kata yang diawali huruf "h" dan diakhiri huruf "o", tekan Ctrl + F lalu ketik h[a-z]*o.



```
micro -plugin install <nama-plugin>
```

plugin install filemanager : Memasang plugin baru.
plugin list : Melihat daftar plugin yang sudah terpasang.
plugin remove filemanager : Menghapus plugin.


Paling Populer untuk Coding & Navigasifilemanager: Menambahkan panel tree-view folder di sisi kiri layar. Sangat berguna untuk melihat struktur file proyek tanpa harus keluar dari Micro.lsp: Menambahkan dukungan Language Server Protocol. Fitur ini membawa fungsi IDE modern seperti auto-completion pintar, melihat definisi fungsi (Alt+D), dan melacak error penulisan kode.jump: Berfungsi melompat langsung ke baris fungsi (function), kelas (class), atau judul bab (heading Markdown) tertentu cukup dengan menekan tombol F4.fzf: Integrasi dengan Fuzzy Finder terminal. Membantu Anda mencari dan membuka file secara instan di dalam folder proyek yang besar hanya dengan mengetikkan fragmen namanya.snippets: Memungkinkan Anda menyisipkan templat kode siap pakai (boilerplate code) sesuai dengan bahasa pemrograman yang sedang digunakan secara otomatis.

