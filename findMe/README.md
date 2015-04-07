# CTF Java HackFest 2015: Find Me!

**Points:** 150
**Author:** 
**Description:**

> Pada soal ini kita mendapatkan kan file yang belum diketahui ekstensinya : 

> ```
begin 644 soal.zip
M4$L#!!0#```(`-
```

> Dari kode diatas, saya mendapatkan clue bahwa file ini harus di decode dengan uudecode, lalu saya coba melakukan decode dan hasilnya saya mendapatkan file soal.zip 

![Alt text](http://i.imgur.com/go2CCRO.png)

> Setelah di ekstract saya mendapatkan sebuah file gambar. 

![Alt text](http://i.imgur.com/caeCUJO.jpg)

> Dari sini saya mencoba untuk melihat metadata gambar tersebut dengan exifttool :

![Alt text](http://i.imgur.com/f0RsYPl.png)

> Dari hasil metadata, saya mendapatkan sebuah enkripsi *eW91IGZpbmQgem9uaw==* yang jika di decode hasilnya “you find zonk”. 

> Lalu saya mencoba membukanya dengan GIMP di linux dan mencoba bermain dengan menu curves pada GIMP dan hasilnya :

![Alt text](http://i.imgur.com/8zd3Kin.png)

> Hasil itu seperti enkripsi base64 tapi jika didecode tidak bisa. perhatikan lagi baik2 pada tulisan itu setelah base64 ada panah menuju angka 13 kita coba menggunakan rot13 ke tulisan itu.. hasilnya *aW5kMG4zczFBX3I0eUE=* , lalu coba kita decode lagi base64 itu dan hasilnya adalah *ind0n3s1A_r4yA*

![Alt text](http://i.imgur.com/8zd3Kin.png)

> Flag : ind0n3s1A_r4yA
