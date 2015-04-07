# CTF Java HackFest 2015: Call Me!

**pass :** javahackfest0x07
**clue :** Event
**point:** 150
**Author:** Gendhenk
**Description** :173.192.181.163:5432 

> Disini saya mendapatkan clue :

```python
def flag(k,l):
	if k=="*" and l=="*":
                return "Flag"
        else:
             	return "Coba lagi gan :D"

regis.register_function(flag,'fl4g')
```
> Setelah berlama-lama googling saya menemukan bahwa soal ini adalah XMLRPC Server dari python, terlihat fungsi *register_function*

> Clue tersebut sama seperti di website ini : 

<https://docs.python.org/2/library/simplexmlrpcserver.html>

> Nah setelah mempelajari web tersebut saya mendapatkan cara untuk memanggil method tersebut. Dari soal tersebut terdapat clue : *Event* ,dimana event tersebut adalah **java hackfest**, lalu saya memanggir method flag alias fl4g dengan parameter "Java" dan "Hackfest" :

```python
import xmlrpclib

s = xmlrpclib.ServerProxy('http://173.192.181.163:5432')
print s.fl4g("Java", "Hackfest")
```
> Tapi hasilnya "Coba lagi gan :D"

Apa yang salah ya? ,ternyata saya coba-coba untuk mengubah clue Java HackFest menjadi lowercase semua :

```python
import xmlrpclib

s = xmlrpclib.ServerProxy('http://173.192.181.163:5432')
print s.fl4g("java", "hackfest")
```
> Dan hasilnya kita langsung mendapatkan flag :

> Flag : congratz_k4mu_j0ss_g4n
