# CTF Java HackFest 2015: Call Me!

**point:** 200
**Author:** Ph4nt0m
**Description** : Clue1 : "Demo Site" | Clue2 : Key = makobu

> Disini saya tidak bisa menjabarkan secara detail beserta Screenshoots karena ketika saya membuat writeup ini saya mencoba melakukan akses ke server soal akan tetapi tidak bisa ,entah dimatikan atau sedang down. Saya jelaskan alur bagaimana saya mendapatkan flagnya.

> Ketika waktu kemarin saya akses saya mencoba malukan CTRL+U / View Source, disitu saya mendapatkan informasi yaitu **id-content**, seperti wordpress yang dirubah prefixnya wp dengan id.

> Kemudian saya mencoba tebak-tebak berhadiah dengan melakukan pengaksesan ke <http://173.192.181.163/soal/gettheflag/id-admin>

> Saya mendapatkan login page nya, kemudian saya coba CTRL+U lagi dan kali ini saya mendapatkan informasi info.txt

> Ketika saya coba mengakses yang beralamatkan <http://173.192.181.163/soal/gettheflag/info.txt> saya mendapatkan informasi username dan password untuk loggin. Seingat saya kalau tidak salah adalah username:admin dan password:billing2015

> Berhasil login dan mencoba keberentungan lagi dengan cara CTRL+U, dan dengan mencoba CTRL+F saya cari kata FLAG dan saya mendapatkan pesan y4L4x673q1, namun ketika saya submit flag tersebut ternyata salah :(

> Entah emang jebakan atau apa, namun selang beberapa saat panitia memberikan clue yaitu key : makobu

> Berawal dari sini saya berpikir bahwa tadi adalah flag yang dienkripsi menggunakan vigenere chiper dengan key makobu. Saya mendapatkan flagnya yaitu m4L4n673c1.

![Alt text](http://i.imgur.com/yMzLnm2.png)
