# CTF Java HackFest 2015: Crx001

**Points:** 50
**Author:** Gendhenk
**Pass :** javahackfest0x01
**Description:**

> Pada soal ini saya mendapatkan file zip, lalu saya extract :

> Lalu saya mendapat sebuah file yang aneh, kita cek dengan perintah :

> **$ file Crypt100**

> Crypt100: XZ compressed data

> File tersebut bertipe XZ, setelah googling, saya mendapatkan cara untuk extract dengan

> perintah :

> $ xz -dc <Crypt100 > crypt

> Kemudian saya mendapatkan sebuah file dengan format tar Lalu ekstrak dan hasilnya kita mendapatkan program executable. Setelah meneliti satu-satu pada folder Crypt100 terdapat file libclu1.0.so yang berisi string :

> **“Hidden clue”**

> Dari sini saya bingung maksudnya apa? Lalu saya coba tekan CTRL + h pada linux dan saya mendapatkan sebuat file tersembunyi yang berisi :

> **“Suppoter Arema Chronous”**

> Dari hasil googling kemungkinan jawabannya adalah :

> * Arema
> * Aremania
> * Aremanita

> Lalu saya mencoba menjalankan lagi file executable tersebut dan saya isikan clue Aremania. 

![Alt text](http://i.imgur.com/c9zZovU.png)

> Tapi aneh, karena apapun input yang kita masukkan pasti akan error, namun saya mendapat clue lagi pada program tersebut yaitu “<string>”, Lalu saya coba lagi dengan menggunakan tanda petik karena string ditulis dengan tanda petik "Aremania" Hasil nya saya mendapatkan sesuatu yang saya curigai flag :

![Alt text](http://i.imgur.com/MBSDQsV.png)

> sy4t:w4in_u4pxs3fg_z4a1s3fg0

> Saya kirim tapi bukan flag. Saya curiga enkripsi tersebut adalah ROT13, setelah saya coba dengan hackbar hasilnya saya mendapatkan flag

![Alt text](http://i.imgur.com/PU3pXIw.png)

> fl4g:j4va_h4ckf3st_m4n1f3st0
