# CTF Java HackFest 2015: Call Me!

**pass :** javahackfest0x06
**point:** 50
**Author:** Gendhenk
**Description** :173.192.181.163:5432 

> Disini kita diberi file executable dimana jika dijalankan maka akan muncul tulisan berjalan yang sangat cepat -_-. 

![Alt text](http://i.imgur.com/W8zhqUM.png)

> Saya pun bingung ini maksudnya minta apa?. Lalu setelah saya perhatikan, tulisan yang berjalan tersebut terdapat jeda. Akhirnya saya kepikiran tulisan tersebut saya simpan di file txt

```
$./game > hasil.txt
```

Setelah disimpan di hasil.txt kata-katanya sangat panjaaang. Saya terus mencari-cari dan akhirnya saya mendapatkan sesuatu yang aneh di tengah-tengah tulisan yang saya curigai adalah flag : 

![Alt text](http://i.imgur.com/IeCK0EH.png)

> Nah setelah kata fl49 ini saya mendapatkan hasil : **W3L_C0_M3_T0_4R_3M4_3R00**. Namun setelah di kirim ternyata ini bukan flag. Lalu saya coba lagi dengan huruf keci, **w3l_c0_m3_t0_4r_3m4_3r00** dan benar ternyata itu adalah flagnya. 

> Flag : w3l_c0_m3_t0_4r_3m4_3r00
