# CTF Java HackFest 2015: Call Me!

**pass :** javahackfest0x06
**point:** 50
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
> Setelah berlama-lama googling saya menemukan bahwa soal ini adalah XMLRPC Server dari python, terlihat dari fungsi yang di register 

```python
regis.register_function(flag,'fl4g')
```

> Clue tersebut sama seperti di website ini : 

<https://docs.python.org/2/library/simplexmlrpcserver.html>

Nah setelah mempelajari web tersebut saya mendapatkan cara untuk memanggil method tersebut. Dari soal tersebut terdapat clue : *Event* ,diana event tersebut adalah java hackfest, lalu saya memanggil method flag alias fl4g dengan parameter java dan hackfest seperti di bawah ini :

```python
import xmlrpclib

s = xmlrpclib.ServerProxy('http://173.192.181.163:5432')
print s.fl4g("java", "hackfest")
```
> Dan hasilnya saya mendapatkan flag : 

> Flag : congratz_k4mu_j0ss_g4n
