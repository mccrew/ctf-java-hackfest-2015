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
> Setelah berlama-lama googling saya menemukan bahwa soal ini adalah XMLRPC Server dari python, terlihat fungsi *register_functio*n
