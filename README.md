# PORT SWIGGER NOTLARI


### LAB Notlarim:

__________________________________________
####  Username enumeration via response timing  [ Response timing ve response received ]

Burada oncelikle ```X-Forwarded-For:``` header i ekleyerek en alta ```0 - 600``` e kadar bir brute force ayarliyorum
ardindan parolayi bilerek yanlis yapiyorum ```testtttttttttttttttttt``` gibi bir parola koyuyorum.
username kismina ise wordlistimi ekleyerek pitchfork ile atagi baslatiyorum. receive ve response timing ile bakarak hani ilk bos bir sorgu gonderiyor
o sorgu senin kendi olusturdugun gercek bir hesabin dogru sifresi ve username i olsun. ondan referans almistim ben.

2054 olarak bos bir istek attiginda yani gercek giris yaptiginda bu sayi ile referansimizi aliyoruz.
username salidirisi bittigi zaman baktigimiz zaman bu 2 parametreye receive ve response timing e . 
Cok ama cok yakin bir deger goruoruz. username i bulmus olduk.
simdi ayni sekilde bu sefer parolaya ayni saldiriyi gerceklestiriyoruz.
saldiri bittiginde gordugumuz deger gercek degerdir.

_______________________________________________________________
