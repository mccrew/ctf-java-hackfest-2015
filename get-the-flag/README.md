# CTF Java HackFest 2015: Get The Flag

**Points:** 80
**Author:** Gendhenk
**Pass :** javahackfest0x04
**Description:**

> Arief adalah seorang karyawan di sebuah perusahaan IT. Ketika sedang bekerja, Arief kemudian mendapat tugas baru untuk mengambil informasi-informasi penting berupa text yang ada di website linux.com. Hasilnya dia mendapatkan ilmu pengetahuan baru tentang pengembangan open source. Setelah membaca artikel-artikel pada web tersebut, ia tertarik untuk mengembangkan aplikasi open source.

> Clue : "Try for digging and get the flag"

Dari clue diatassaya mendapat informasi tentang dig dan TXT. Pada linux
terdapat menu dig, lalu saya coba dengan arguman TXT

$ dig +short TXT linux.com

Kemudian saya mendapatkan hasil :
$ dig +short TXT linux.com

"google-site-verification=SDW6U9788xC80xinO4aDxrgD4bkaCjLozXPv4R7oMbk"
"v=spf1 mx +all"
"google-site-verification=AqV3SU_MRUY0GYnNYAKi_6pa0S1WU7hfq5SapcMUycI"

Lalu saya mencoba untuk mengirimkan “ SDW6U9788xC80xinO4aDxrgD4bkaCjLozXPv4R7oMb” dan ternyata benar, itu adalah
flagnya :D

> Flag : SDW6U9788xC80xinO4aDxrgD4bkaCjLozXPv4R7oMb

