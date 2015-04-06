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

> Lalu saya mencoba menjalankan lagi file executable tersebut lalu saya isikan clue :
