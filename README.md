```python
            # VERİ TİPLERİ

 ########################################################################################################################################
 ###    Tip     ###  Kisaltma  ###             Örnek           ###                     Açıklama                                       ###
 ### --------------------------------------------------------- ###--------------------------------------------------------------------###
 ###  Integer   ###    int     ###             3, 10           ###     Tam Sayı                                                       ###
 ###   Float    ###   float    ###            1.5, 7.0         ###     Ondalıklı Sayı                                                 ###
 ###   String   ###    str     ###           "S3m", '2'        ###     Yazı                                                           ###
 ###  Boolean   ###    bool    ###          True, False        ###     Mantıksal İşlemler                                             ###
 ###    List    ###    list    ###      [1,2,True, 'a', 1]     ###     Hem tekrar edebilen hemde farklı veri tiplerini içeren tiptir  ###
 ###    Set     ###    set     ###         {1,2,True, 'a'}     ###     List tipinden farkı tekrarlanamaz                              ###
 ### Dictionary ###    dict    ### {'isim': 'Mesut, 'yas': 32} ###     Anahtar ve buna karşılık gelen değerlerdir                     ###
 ###    Tuple   ###    tup     ###         (1, 2, True)        ###     List tipinden farkı parantez içerisine yazılanlar değişmez     ###
 ######################################################################################################################################## 
```


```python

```

## SAYI VERİ TİPLERİ


```python
print (2+2)
```

    4
    


```python
print (2+5.2)
```

    7.2
    


```python
print (type (2)) #Veri tipinin hangi tipte olduğunu öğrenmek için type komutu kullanılır.
```

    <class 'int'>
    


```python
print (type(5.2))
```

    <class 'float'>
    


```python
print (2**3) #Sayının üssünü alır.
```

    8
    


```python
print (10%2) #Modunu alır ve kalanı verir.
```

    0
    


```python
print (10/3)
```

    3.3333333333333335
    


```python
print (10//3) #Tam kısmını verir virgülden sonrasını almaz.
```

    3
    


```python

```

### DEĞİŞKEN TANIMLAMA KURALLARI
    # Kabul edilmeyen degisken isim atama senaryolari:
    # * sayi ile baslamak
    # * bosluk icermek
    # * "*(/ gibi semboller icermek
    # * rezerve edilmis isimleri kullanmak


```python
maasAli = 5000
maasAhmet = 4000
vergi = 0.27

print (maasAli- (maasAli * vergi))
print (maasAhmet- (maasAhmet * vergi))
print (5000 - (5000 * 0.27))
print (4000 - (4000 * 0.27))
```

    3650.0
    2920.0
    3650.0
    2920.0
    


```python
number1 = 20
number1 += 30 # number1 = number1 + 30 anlamına gelir
print (number1)
```

    50
    


```python
x = 1
y = 2.3
name = "Mecit"
isStudent = True
```


```python
x, y, name, isStudent = (1,2.3,"Mecit", True)
```


```python
a = 10
b = 20 
print (a+b) #30
```

    30
    


```python
m = '10'
t = '20'
print (m+t) #1020
```

    1020
    


```python
firstname = "Mecit"
lastname = "Türkmen"
print (firstname + ' ' +lastname)
```

    Mecit Türkmen
    


```python

```

## QUİZ


```python
# 1- Bir müşterinin aşağıdaki bilgileri için değişken oluşturunuz.

# Müşteri adı
# Müşteri soyadı
# Müşteri ad+soyad
# Müşteri cinsiyet
# Müşteri tc kimlik no
# Müşteri doğum yılı
# Müşteri adres bilgisi
# Müşteri yaşı
```


```python
musteriAdı = 'Mecit'
musteriSoyadı = 'Türkmen'
musteriAdSoyad = musteriAdı + ' ' + musteriSoyadı
musteriCinsiyet = 'Erkek'
musteriTc = 11111111111
musteriDogum = 1997
musteriAdres = 'ilkadım/Samsun'
musteriAge = 26

print (musteriAdı)
print (musteriSoyadı)
print (musteriAdSoyad)
print (musteriCinsiyet)
print (musteriTc)
print (musteriDogum)
print (musteriAdres)
print (musteriAge)
```

    Mecit
    Türkmen
    Mecit Türkmen
    Erkek
    11111111111
    1997
    ilkadım/Samsun
    26
    


```python
# 2- Aşağıdaki siparişlerin toplam bilgisini hesaplayınız.

#       Sipariş 1 => 110    TL
#       Sipariş 2 => 1100.5 TL
#       Sipariş 3 => 356.95 TL
```


```python
sıparıs1 = 110
sıparıs2 = 1100.5
sıparıs3 = 356.95
toplam = sıparıs1 + sıparıs2 + sıparıs3
print (toplam)
print (sıparıs1 + sıparıs2 + sıparıs3)
```

    1567.45
    1567.45
    


```python

```

## VERİ TİP DÖNÜŞÜMLERİ


```python
'''
x = int (input ('1.sayı: ')) #Başına int konulmaz ise string tipi olarak algılar
y = int (input ('2.sayı: '))
toplam = x + y
print (toplam)
'''
```




    "\nx = int (input ('1.sayı: ')) #Başına int konulmaz ise string tipi olarak algılar\ny = int (input ('2.sayı: '))\ntoplam = x + y\nprint (toplam)\n"




```python
x = 5               #int
y = 2.5             #float
name = "Mecit"      #string
isOnline = True    #boolean
```


```python
# int to float
x = float(x)
print(x)       # x = 5.0 olur yani float oldu.
print(type(x))  # ctrl + k + u yorum satırını tam tersine çevirir.
```

    5.0
    <class 'float'>
    


```python
 # float to int
y = int(y)
print(y)       # y = 2 olur yani int oldu. Ondalıklı kısmını siler.
print (type (y))
```

    2
    <class 'int'>
    


```python
result = x + y
print (result)
print(type (result))
```

    7.0
    <class 'float'>
    


```python
#bool to str
isOnline = str (isOnline)
print (isOnline)
print(type(isOnline))
```

    True
    <class 'str'>
    


```python
#bool to int
isOnline = int(isOnline)
print (isOnline)       #True mantıkta 1 , false mantıkta 0 anlamına gelir.
print (type(isOnline))
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    Cell In[19], line 2
          1 #bool to int
    ----> 2 isOnline = int(isOnline)
          3 print (isOnline)       #True mantıkta 1 , false mantıkta 0 anlamına gelir.
          4 print (type(isOnline))
    

    ValueError: invalid literal for int() with base 10: 'True'



```python
#Soru:  Daire Alanı : π r²
#       Daire Çevresi: 2πr
# Yarı çapı bilgisi kullanıcıdan alınan bir dairenin alanı ve dairesini hesaplayınız. (r:3.14)
```


```python
pi = int (input('pidegeri= '))
r = float (input('yarıçap= '))
dairealan1 = pi*(r**2)
dairecevre1= 2*pi*r
print (dairealan1)
print (dairecevre1)
```

    pidegeri=  3
    yarıçap=  2
    12.0
    12.0
    


```python

```

## STRİNG VERİ TİPLERİ


```python
name = 'Mecit'
surname = 'Türkmen'
age = 25
print ('My name is '+ name +' '+ surname)
```

    My name is Mecit Türkmen
    


```python
greeting ='My name is '+ name +' '+ surname + ' and \nI am '+ str(age) + ' years old.' #\n ile alt satıra geçirilir # age ifadesi str tipine dönüştürlmez ise hata verecektri str ile str toplanır.
```


```python
print (greeting [0])
print (greeting [3])

print (len (greeting)) #Bir ifadenin uznluğu için len komutu kullanılır.
```

    M
    n
    48
    


```python
print (greeting [47])
print (greeting [3:7]) #3ten başla7 ye kadar git 7 dahil değil
print (greeting [2:40:2]) #2den başla 40 dahil değil 2 karakterde bir al
```

    .
    name
     aei ei üke n Ia 5y
    


```python
print('Benim adım {}, soyadım{}'.format('mecit',' türkmen')) #Format değişkeni ile değişken atama yapılır.
print('Benim adım {1}, soyadım{0}'.format('mecit',' türkmen'))
```

    Benim adım mecit, soyadım türkmen
    Benim adım  türkmen, soyadımmecit
    


```python
result = 200/700
print ('the result is {}'.format ( result))
print ('the result is {r:1.3}'.format (r=result)) #virgülden sonra 3 basamak
print ('the result is {r:10.3}'.format (r=result)) #virgülden önce 10 karakterlik olacak
```

    the result is 0.2857142857142857
    the result is 0.286
    the result is      0.286
    


```python
name = 'mecit'
surname = ' türkmen'
print(f"Benim adım {name}, soyadım {surname}") #tırnak başına f ekleyerekde format fonksiyonu aktif olmaktadır.
```

## QUİZ


```python
website ="http://www.sadikturan.com"
course = "Python Kursu : Baştan Sona Python Programlama Rehberiniz (40 saat)"
```


```python
# 1- 'course' karakter dizisinde kaç karakter bulunmaktadır?

print (len(course))
```

    66
    


```python
# 2- 'website' içinden www karakterlerini alın.

print (website [7:10])
```

    www
    


```python
# 3- 'website' içinden com karakterilerini alın.

print (website [22:])  #veya print (website [length-3:lenght])
```

    com
    


```python
# 4- 'course' içinden ilk 15 ve son 15 karakterlerini alın.

print (course [:15])
print (course [-15:])
```

    Python Kursu : 
    riniz (40 saat)
    


```python
# 5- 'course' ifadesindeki karakterleri tersten yazdırın.

print (course [::-1]) #-1 yazarak bütün karakterleri ters yazdırır.
```

    )taas 04( zinirebheR amalmargorP nohtyP anoS natşaB : usruK nohtyP
    


```python
name, surname, age, job = 'Bora' , 'Yılmaz' , 32 , 'Mühendis'
```


```python
# 6- Yukarıda verilen değişkenler için ekrana aşağıdaki ifadeyi yazdırın.
#   'Benim adım Bora Yılmaz, Yaşım 32 ve mesleğim Mühendis.'

print ('Benim adım {}, Yaşım {} ve mesleğim {}'.format ((name + ' ' + surname), age, job))
```

    Benim adım Bora Yılmaz, Yaşım 32 ve mesleğim Mühendis
    


```python
# 7- 'Hello world' ifadesindeki w harfini 'W' ile değiştirin.

s = 'Hello world'
s = s[0:6] + 'W' + s[-4:]
print (s)

#veya

s.replace ('w', 'W') #replace ile değişim işlemi yapılabilir.
print (s)
```

    Hello World
    Hello World
    


```python
# 8- 'abc' ifadesini yan yana 3 defa yazdırınız.

print ('abc'*3)
```

    abcabcabc
    


```python

```

## STRİNG METOTLARI


```python
message = 'Hello There. My name is Mecit Türkmen'
```


```python
message = message.upper() #message değişkeni içerisindeki her harfi büyük harf yapar.
print (message)
```

    HELLO THERE. MY NAME IS MECIT TÜRKMEN
    


```python
message = message.lower() #message değişkeni içerisideki her harfi küçük harf yapar.
print (message)
```

    hello there. my name is mecit türkmen
    


```python
message = message.title() #message değişkeni içerisindeki her kelimenin ilk harfini büyük harf yapar.
print (message)
```

    Hello There. My Name Is Mecit Türkmen
    


```python
message = message.capitalize() #message değişkeni içerisinde sadece ilk kelimenin ilk harfini büyük harf geri kalanını küçük harf yapar.
print (message)
```

    Hello there. my name is mecit türkmen
    


```python
message1 = ' Hello There. My name is Mecit Türkmen'
message1 = message1.strip() #message1 değişkeni içerisindeki ifadenin başında veya sonunda eğer boşluk karakteri varsa bunu siler.
print (message1)
```

    Hello There. My name is Mecit Türkmen
    


```python
message = message.split() #message değişkeni içersindeki cümleyi liste tipine çevirmek için kullanılır.
print (message)
```

    ['Hello', 'there.', 'my', 'name', 'is', 'mecit', 'türkmen']
    


```python
message = ' '.join(message) #split ile ayrılmış bir ifadeyi join ile birleştirebiliriz. 
#Boşluk konulma sebebi birleştirilen ifade arasında boşluk olsun diye.
print (message)
```

    H e l l o   t h e r e .   m y   n a m e   i s   m e c i t   t ü r k m e n
    


```python
index = message.find('mecit') #Bir cümle içerisinde bulmak istenilen kelimenin ilk harfinin index numarasını verir.
#(-1) değeri gelirse bu kelimenin olmadığı anlamına gelir.
print (index)
```

    -1
    


```python
isFound = message.startswith ('H') #Cümle 'H' ile başlayıp başlamadığının sorgusudur.
print (isFound)
```

    True
    


```python
isFound = message.endswith ('n') #Cümle 'n' ile bitip bitmediğinin sorgusudur.
print (isFound)
```

    True
    


```python
message = message.replace('mecit','Mecit') #replace komutu cümle içerisinde yer alan 'mecit' kelimesini arar sonra yazılması 
#istenilen 'Mecit' kelimesini yazar.
print (message)
```

    H e l l o   t h e r e .   m y   n a m e   i s   m e c i t   t ü r k m e n
    


```python
message = message.center(50,'*') #message değişkenin 100 karakterli olmasını ister. 
#center 100 karakter olması için ifadenin başında ve sonunda eşit şekilde boşluk bırakır. 
#virgül ile ayırıp boşluk kısmına istenilen ifadede yazılabilir.
print(message)
```

    H e l l o   t h e r e .   m y   n a m e   i s   m e c i t   t ü r k m e n
    


```python
message = message.count ('a') #message değişkeni içerisinde kaç tane a olduğunu gösterir.
print (message)
```

    1
    


```python

```

## QUİZ


```python
website = "http://www.sadikturan.com"
course  = "Python Kursu: Baştan Sona Python Programlama Rehberiniz (40 saat)"
```


```python
# 1-    ' Hello world ' karakter dizisinin baş ve sondaki boşluk karakterini silin.

x = ' Hello world '
x = x.strip()
print (x)
```

    Hello world
    


```python
# 2-    'www.sadikturan.com' içindeki sadikturan bilgisi harcindeki her karakteri silin.

y = 'www.sadikturan.com'
y = y.replace('www.','').replace('.com','')
print (y)
```

    sadikturan
    


```python
# 3-    'course' karakter dizisinin tüm karakterlerini küçük harf yapın.

course = course.lower ()
print (course)
```

    python kursu: baştan sona python programlama rehberiniz (40 saat)
    


```python
# 4-    'website' içinde kaç tane a karakteri vardır? (count('a))

website = website.count ('a')
print (website)

```

    2
    


```python
# 5-    'website' 'www' ile başlayıp 'com' ile bitiyor mu?

website = "http://www.sadikturan.com"
sorgu1 = website.startswith ('www')
print (sorgu1)

sorgu2 = website.endswith ('com')
print (sorgu2)
```

    False
    True
    


```python
# 6-    'website' içinde '.com' ifadesi var mı?

website = "http://www.sadikturan.com"
result = website.find ('.com')
print (result)

result = website.rfind ('.com') #sondan başlayarak arar.
print (result)
```

    21
    21
    


```python
# 7-    'course' içindeki karakterlerin hepsi alfabetik mi? (isaplha, isdigit)

result1 = course.isalpha()
print (result1)

result2 = course.isdigit ()
print (result2)
```

    False
    False
    


```python
# 8-    'Contents' ifadesini satırda 50 karakter yapıp sağ ve soluna '*' koyunz.

result3 = 'Contents'.center(50,'*')
print (result3)

result4 = 'Contents'.rjust(50,'*') #sağına yıldız ekler
print (result4)

result5 = 'Contents'.ljust(50,'*') #soluna yıldız ekler.
print (result5)
```

    *********************Contents*********************
    ******************************************Contents
    Contents******************************************
    


```python
# 9-    'course' içindeki tüm boşluk karakterlerini '-' ile değiştirin.

course  = "Python Kursu: Baştan Sona Python Programlama Rehberiniz (40 saat)"

result6 = course.replace (' ','-')
print (result6)
```

    Python-Kursu:-Baştan-Sona-Python-Programlama-Rehberiniz-(40-saat)
    


```python
# 10-   'Hello Wolrd' ifadesindeki 'world' yerine 'there' yazınız.

result7 = 'Hello World'.replace('World','there')
print (result7)
```

    Hello there
    


```python
# 11-   'course' ifadesini boşluk karakterlerinden sonra ayırın.

course  = "Python Kursu: Baştan Sona Python Programlama Rehberiniz (40 saat)"
result8 = course.split (' ')
print(result8)
```

    ['Python', 'Kursu:', 'Baştan', 'Sona', 'Python', 'Programlama', 'Rehberiniz', '(40', 'saat)']
    


```python

```

## Liste Veri Tipi


```python
message= 'Hello There. My name is Mecit Türkmen'.split()
print (message)
print (message[0]) #Liste tipinde index bulunmak için kullanılır.
```

    ['Hello', 'There.', 'My', 'name', 'is', 'Mecit', 'Türkmen']
    Hello
    


```python
my_list = [1,2,3]
print(my_list)
```

    [1, 2, 3]
    


```python
my_list1 = ['bir',2,True,5.6]
print (my_list1)
```

    ['bir', 2, True, 5.6]
    


```python
#Listelerde Toplama işlemi
```


```python
list1 = ['one', 'two', 'three']
list2 = ['four', 'five', 'six']
numbers = list1 + list2
print (numbers)
```

    ['one', 'two', 'three', 'four', 'five', 'six']
    


```python
print (len(numbers)) #Karakterin uzunluğunu bulmak için kullanılır.
```

    6
    


```python
userA = ['mecit' , 35]
userB = ['kübra' , 26]
users = userA + userB
print (users)
```

    ['mecit', 35, 'kübra', 26]
    


```python
#Liste içinde Liste oluşturmak için ise;
```


```python
users1 =  [userA, userB]
print (users1)
print (users1 [1])

a = users1 [1]
print (a[0])
print (users1 [0][1])
```

    [['mecit', 35], ['kübra', 26]]
    ['kübra', 26]
    kübra
    35
    


```python

```

## QUİZ


```python
#1- "BMW, Mercedes, Opel, Mazda" elemanlarına sahip bir liste oluşutrunuz.

car = ["BMW", "Mercedes", "Opel", "Mazda"]
print (car)
print (type (car))
```

    ['BMW', 'Mercedes', 'Opel', 'Mazda']
    <class 'list'>
    


```python
#2- Liste kaç elemanlıdır?

print (len(car))
```

    4
    


```python
#3- Listenin ilk ve son elemanı nedir?

print (car[0])
print (car [3])

```

    BMW
    Mazda
    


```python
#4- Mazda değerini Toyota ile değiştirin.

car [-1] = 'Toyota'
print (car)
```

    ['BMW', 'Mercedes', 'Opel', 'Toyota']
    


```python
#5- Mercedes listenin bir elemanı mıdır?

result = 'Mercedes' in car
print (result)
```

    True
    


```python
#6- Listenin -2 indeksindeki değer nedir?

result1 = car [-2]
print (result1)

```

    Opel
    


```python
#7- Listenin ilk 3 elemanını alınız.

result2 = car[0] + ' ' + car[1] + ' ' + car[2]
print (result2)

result3 = car [0:3]
print (result3)
```

    BMW Mercedes Opel
    ['BMW', 'Mercedes', 'Opel']
    


```python
#8- Listenin son 2 elemanı yerine "Toyota" ve "Renault" değerini girin.

car[3] = 'Renault'
car[2] = 'Toyota'
print (car)

car [-2:] = ['Toyota' , 'Renault']
print (car)

```

    ['BMW', 'Mercedes', 'Toyota', 'Renault']
    ['BMW', 'Mercedes', 'Toyota', 'Renault']
    


```python
#9- Listenin üzerine "Audi" ve "Nissan" değerlerini ekleyin.

result4 = car + ['Audi'] + ['Nissan']
print (result4)
```

    ['BMW', 'Mercedes', 'Toyota', 'Renault', 'Audi', 'Nissan']
    


```python
#10- Listenin son elemanını siliniz.

result4 = car + ['Audi'] + ['Nissan']
print (result4 [0:5])
```

    ['BMW', 'Mercedes', 'Toyota', 'Renault', 'Audi']
    


```python
#11- Liste elemanlarını tersten yazdırınız.

print (result4[::-1])
```

    ['Nissan', 'Audi', 'Renault', 'Toyota', 'Mercedes', 'BMW']
    


```python
#12-  Aşağıdaki verileri bir liste içinde saklayınız.

        # studentA: Yiğit Bilgi 2010, (70,60,70)
        # studentB: Sena Turan 1999, (80,80,70)
        # studentC: Ahmet Turan 1998, (80,70,90)

studentA = ['Yiğit', 'Bilgi', 2010, (70,60,70)]
print (studentA)

studentB = ['Sena', 'Turan', 1999, (80,80,70)]
print (studentB)

studentC = ['Ahmet', 'Turan', 1998, (80,70,90)]
print (studentC)

students = [studentA] + [studentB] + [studentC]
print (students)
```

    ['Yiğit', 'Bilgi', 2010, (70, 60, 70)]
    ['Sena', 'Turan', 1999, (80, 80, 70)]
    ['Ahmet', 'Turan', 1998, (80, 70, 90)]
    [['Yiğit', 'Bilgi', 2010, (70, 60, 70)], ['Sena', 'Turan', 1999, (80, 80, 70)], ['Ahmet', 'Turan', 1998, (80, 70, 90)]]
    


```python
#13-  Liste elemanlarını ekrana yazdırınız.

name = studentA [0]
surname = studentA [1]
dogumyılı = studentA [2]
puanı = studentA [3]

print (name)
print (surname)
print (dogumyılı)
print (puanı)

```

    Yiğit
    Bilgi
    2010
    (70, 60, 70)
    


```python

```

## Liste Veri Tipi Metotları


```python
numbers = [1, 10, 5, 16, 4, 9 ,10]
letters = ['a', 'g', 's', 'b', 'y', 'a', 's']
```


```python
val = min(numbers) #min komutu numbers içerisindeki en düşük sayıyı gösterir.
print (val)
```

    1
    


```python
val2 = max(numbers) #max komutu numbers içerisindeki en büyük sayıyı gösterir.
print (val2)
```

    16
    


```python
val3 = min(letters) #alfabetik sıraya göre ilk harf
print (val3)
```

    a
    


```python
val4 = max (letters) #alfabetik sıraya göre son harf
print (val4)
```

    y
    


```python
val5 = numbers [3:6] #string metodunda olduğu gibi kısıtlamalar yapılabilir.
print (val5)
```

    [16, 4, 9]
    


```python
val6 = letters [4:]
print (val6)
```

    ['y', 'a', 's']
    


```python
numbers [4] = 40 #Belirtilen indexdeki elemanı değiştirmek için kullanılır.
print (numbers)
```

    [1, 10, 5, 16, 40, 9, 10]
    


```python
numbers.append(59) #append komutu parantez içersine yazılan ifadeyi listenin sonuna eklenir.
print (numbers)
```

    [1, 10, 5, 16, 40, 9, 10, 59]
    


```python
numbers.insert(3,78) #insert komutu ile istenilen indexe istenilen sayı atanır. O indexteki elemanı silmez!!!
print (numbers)
```

    [1, 10, 5, 78, 16, 40, 9, 10, 59]
    


```python
numbers.insert (-1,52) #en son index numarasından önce elemanı ekler.
print (numbers)
```

    [1, 10, 5, 78, 16, 40, 9, 10, 52, 59]
    


```python
numbers.pop() #İçi boş ise son elemanı siler. Parantez içerisine index numarası yazarsak o indexteki elemanı siler.
print(numbers)
```

    [1, 10, 5, 78, 16, 40, 9, 10, 52]
    


```python
numbers.remove (52) #Belirtilen elemanı siler.
print (numbers)
```

    [1, 10, 5, 78, 16, 40, 9, 10]
    


```python
numbers.sort () #sayısal olarak sıralar
print (numbers)
```

    [1, 5, 9, 10, 10, 16, 40, 78]
    


```python
letters.sort () #alfabetik olarak sıralam yapar.
print (letters)
```

    ['a', 'a', 'b', 'g', 's', 's', 'y']
    


```python
numbers.reverse () #büyükten küçüğe sıralar.
print (numbers)
```

    [78, 40, 16, 10, 10, 9, 5, 1]
    


```python
letters.reverse () #alfabetik olarak zden a ya sıralar.
print (letters)
```

    ['y', 's', 's', 'g', 'b', 'a', 'a']
    


```python
print (len(numbers))  #liste içindeki eleman sayısını verir
print (len(letters))
```

    8
    7
    


```python
print (numbers.count(10)) #liste içinde o elemandan kaç adet olduğun gösterir.
print (letters.count('a'))
```

    2
    2
    


```python
numbers.clear() #liste içindeki tüm elemanları siler.
print (numbers)
```

    []
    


```python

```

## QUİZ


```python
names = ['Ali', 'Yağmur', 'Hakan', 'Deniz']
years = [1998, 2000, 1998, 1987]
```


```python
# 1-    "Cenk" ismini listenin sonuna ekleyiniz.

names = ['Ali', 'Yağmur', 'Hakan', 'Deniz']
names.append ('Cenk')
print (names)

```

    ['Ali', 'Yağmur', 'Hakan', 'Deniz', 'Cenk']
    


```python
# 2-    "Sena" değerini listenin başına ekleyiniz.

names.insert (0, 'Sena')
print (names)

```

    ['Sena', 'Ali', 'Yağmur', 'Hakan', 'Deniz', 'Cenk']
    


```python
# 3-    "Deniz" değerini listeden siliniz.

names.pop (3)
print (names)
```

    ['Sena', 'Ali', 'Yağmur', 'Deniz', 'Cenk']
    


```python
# 4-    "Deniz" değerinin indexi nedir?

names = ['Ali', 'Yağmur', 'Hakan', 'Deniz']
print (names.index ('Deniz'))
```

    3
    


```python
# 5-    'Ali' listenin bir elemanı mıdır?

result1 = 'Ali' in names
print (result1)

result2 = 'Ali' in years
print ( result2)
```

    True
    False
    


```python
# 6-    Liste elemanlarını ters çevirin.

print (names [::-1])
print (years [::-1])
```

    ['Deniz', 'Hakan', 'Yağmur', 'Ali']
    [1987, 1998, 2000, 1998]
    


```python
# 7-    Liste elemanlarını alfabetik olarak sıralayın.

names.sort ()
print (names)
```

    ['Ali', 'Deniz', 'Hakan', 'Yağmur']
    


```python
# 8-    years listesindeki rakamsal olarak sıralayın.

years.sort()
print (years)

years.reverse ()
print (years)
```

    [1987, 1998, 1998, 2000]
    [2000, 1998, 1998, 1987]
    


```python
# 9-    str = "Chevrolet,Dacia" karakter dizisini liste tipine çevirin.

str  = ['Chevrolet', 'Dacia']
print (str)
print (type (str))
```

    ['Chevrolet', 'Dacia']
    <class 'list'>
    


```python
# 10-   years dizisinin en büyük ve en küçük elemanı nedir?

print (min(years))
print (max(years))
```

    1987
    2000
    


```python
# 11-   years dizisinde kaç tane 1998 değeri vardır?

print (years.count (1998))
```

    2
    


```python
# 12-   years disindeki tüm elemanları siliniz.

print (years.clear())
```

    None
    


```python
# 13-   Kullanıcıdan alacağınız 3 tane marka bilgisini bir listede saklayınız.

user1 = list(input('Marka Bilgisini Giriniz: '))
user2 = list(input('Marka Bilgisini Giriniz: '))
user3 = list(input('Marka Bilgisini Giriniz: '))

markalar = user1 + user2 + user3

print (markalar)

#veya 

markalar = []

marka = input ("marka: ")
markalar.append (marka)

marka = input ("marka: ")
markalar.append (marka)

marka = input ("marka: ")
markalar.append (marka)

print (markalar)
```

    Marka Bilgisini Giriniz:  rt
    Marka Bilgisini Giriniz:  rt
    Marka Bilgisini Giriniz:  rt
    ['r', 't', 'r', 't', 'r', 't']
    


```python

```

## Tuple Veri Tipi


```python
list =[1,2,3]

tuple = (1,"iki", 3)

print(type(list))
print(type(tuple))
```

    <class 'list'>
    <class 'tuple'>
    


```python
print (list[2])
print (tuple[2])
```

    3
    3
    


```python
print (len(list))
print (len(tuple)) #Aynı şekilde len fonksiyonu ile uzunluğunu bulabiliriz.
```

    3
    3
    


```python
# Tuple değiştirilemeyen özelliktedir.
tuple[0] = "Deniz"
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[12], line 2
          1 # Tuple değiştirilemeyen özelliktedir.
    ----> 2 tuple[0] = "Deniz"
    

    TypeError: 'tuple' object does not support item assignment



```python
tuple.count(1) #Liste de olduğu gibi count ile kaç tane olduğunu bulabiliriz.
```




    1




```python
tuple.index("iki") # index metodu ise iki strsinin kaçıncı index de olduğunu belirtir.
```




    1




```python
tuple1 = (1,"iki", 3)
tuple2 = (2,"dört", 5)

print (tuple1 + tuple2) #iki tuple birleştirmek için
```

    (1, 'iki', 3, 2, 'dört', 5)
    


```python

```

## Dictionary Veri Tipi


```python
#Bu veri tipi bir anahtar(key) ve bir değerden(value) oluşur.
```


```python
sehirler = ["Kocaeli", "İstanbul"]
plakalar = [41,34]

print (plakalar[sehirler.index("Kocaeli")])
print (plakalar[sehirler.index("İstanbul")])
```

    41
    34
    


```python
# Yukarıdaki örnekte kod uzadığını görüyoruz. Bunun için sözlük veri yapısında yazarsak
```


```python
plakalar = { "Kocaeli" : 41, "İstanbul":34}

print (plakalar["Kocaeli"])
print (plakalar["İstanbul"])
```

    41
    34
    


```python
plakalar["Ankara"] = 6 #Sözlük yapısında veri içerisine tekrar eleman ataması yapılabilir.
```


```python
print (plakalar)
```

    {'Kocaeli': 41, 'İstanbul': 34, 'Ankara': 6}
    


```python
users = {
    "sadıkturan" : 36,
    "cinarturan" :2
}
```


```python
print(users["cinarturan"])
```

    2
    


```python
users = {
    "sadıkturan" : {
        "age" : 36,
        "email" : "sadık@gmail.com",
        "address" : "kocaeli",
        "phone" : "12341234"
    },
    "cinarturan" : {
        "age" : 2,
        "email" : "cinark@gmail.com",
        "address" : "kocaeli",
        "phone" : "01010101"
    }
}
```


```python
print(users["cinarturan"])
```

    {'age': 2, 'email': 'cinark@gmail.com', 'address': 'kocaeli', 'phone': '01010101'}
    


```python
print(users["cinarturan"]["age"])
```

    2
    


```python

```

'''
    ogrenciler = {
        '120': {
            'ad': 'Ali',
            'soyad': 'Yılmaz',
            'telefon': '532 000 00 01'
        },
        '125': {
            'ad': 'Can',
            'soyad': 'Korkmaz',
            'telefon': '532 000 00 02'
        },
        '128': {
            'ad': 'Volkan',
            'soyad': 'Yükselen',
            'telefon': '532 000 00 03'
        },
    }

    1- Bilgileri verilen öğrencileri kullanıcıdan aldığınız bilgilerle
       dictionary içinde saklayınız.

    2- Öğrenci numarasını kullanıcıdan alıp ilgili öğrenci bilgisini gösterin.
'''


```python
ogrenciler = {}

number = input("öğrenci no: ")
name = input("öğrenci adı: ")
surname = input("öğrenci soyad: ")
phone = input("öğrenci telefon: ")

ogrenciler.update({
    number: {
        'ad': name,
        'soyad': surname,
        'telefon':phone 
    }
})
print('*'*50)    
```

    öğrenci no:  120
    öğrenci adı:  Ali
    öğrenci soyad:  Yılmaz
    öğrenci telefon:  532000
    **************************************************
    


```python
ogrNo = input('öğrenci no: ')
ogrenci = ogrenciler[ogrNo]
print(ogrenci)

print(f"Aradığınız {ogrNo} nolu öğrencinin adı: {ogrenci['ad']} soyadı: {ogrenci['soyad']} ve telefonu ise {ogrenci['telefon']}")
```

    öğrenci no:  120
    {'ad': 'Ali', 'soyad': 'Yılmaz', 'telefon': '532000'}
    Aradığınız 120 nolu öğrencinin adı: Ali soyadı: Yılmaz ve telefonu ise 532000
    


```python

```

## Set Veri Tipi


```python
fruits = { 'orange', 'apple', 'banana'}

# print(fruits[0]) indekslenemez
```


```python
for x in fruits:
    print(x)
```

    apple
    orange
    banana
    


```python
fruits.add('cherry') #cherry strinigin küme veri tipine ekler.
fruits
```




    {'apple', 'banana', 'cherry', 'orange'}




```python
fruits.update(['mango','grape','apple']) #birden fazla eleman eklemek için kullanılır.
#Tekrarlanamaz olduğu için tekrarlayan elemanlar çıkartılır.
fruits
```




    {'apple', 'banana', 'cherry', 'grape', 'mango', 'orange'}




```python
fruits.remove('mango') #mango str sini siler.
fruits
```




    {'apple', 'banana', 'cherry', 'grape', 'orange'}




```python
fruits.discard('apple') #apple strsini siler.
fruits
```




    {'banana', 'cherry', 'grape', 'orange'}




```python
fruits.pop() #Herhangi bir elmanı siler.
fruits
```




    {'banana', 'cherry'}




```python
fruits.clear() #Bütün elemanları siler.
fruits
```




    set()




```python

```

## Atamalar


```python
# x = 5
# y = 10
# z = 20

x,y,z = 5,10,20
print (x,y,z)
```

    5 10 20
    


```python
# x, y = y, x Birbiri Arasında değiştirme anlamında
# x += 5          # x = x + 5
# x -= 5          # x = x - 5
# x *= 5          # x = x * 5
# x /= 5          # x = x / 5
# x %= 5          # x = x % 5
# y //= 5         # y = y // 5
# y **= z         # y = y ** z
```


```python
values = 1, 2, 3, 4, 5

print(values)
print(type(values))
```

    (1, 2, 3, 4, 5)
    <class 'tuple'>
    


```python
x, y, *z = values # Anlamı şudur x ve y ilk indeksi alsın.
#z ise geriye kalanları alarak listeye dönüşsün.

print(x, y, z)
print(type(values))
print(x, y, z[1])
```

    1 2 [3, 4, 5]
    <class 'tuple'>
    1 2 4
    


```python

```

## QUİZ


```python
x, y, z = 2, 5, 10
```


```python
# 1- Kullanıcıdan aldığınız 2 sayının çarpımı ile x,y,z toplamının farkı nedir ?

a = int(input("1. Sayıyı Giriniz:"))
b = int(input("2. Sayıyı Giriniz:"))
c = a * b
d = x + y + z
e = c - d

print ("Girmiş olduğunuz Sayıların Çarpımı {}'dir. Aynı zamanda farkları ise {}'dir.".format(c,e))
```

    1. Sayıyı Giriniz: 2
    2. Sayıyı Giriniz: 4
    Girmiş olduğunuz Sayıların Çarpımı 8'dir. Aynı zamanda farkları ise -9'dir.
    


```python
# 2- y' nin  x' e kalansız bölümünü hesaplayınız.

result = y // x
print (result)
```

    2
    


```python
# 3- (x,y,z) toplamının mod 3' ü nedir ?

toplam = (x+ y+ z)
result = toplam % 3
print(result)
```

    2
    


```python
# 4- y' nin x. kuvvetini hesaplayınız.

result = y ** x
print (result)
```

    25
    


```python
# 5- x, *y, z = numbers işlemine göre z' nin küpü kaçtır ?

numbers = 1, 5, 7, 10, 6
x, *y ,z = numbers
result = z ** 3
print(result)
```

    216
    


```python
# 6- x, *y, z = numbers işlemine göre y nin değerleri toplamı kaçtır ?

numbers = 1, 5, 7, 10, 6
x, *y ,z = numbers
result = y[0] + y[1] + y[2]

print(result)
```

    22
    


```python

```

## Karşılaştırma Operatörleri


```python
a, b, c, d = 5, 5, 10, 4
```


```python
password = '1234'
username = 'sadikturan'
```


```python
result = (a == b) # a ile b birbirine eşit mi?
print(result)
```

    True
    


```python
result = (a == c) # a ile c birbirine eşit mi?
print(result)
```

    False
    


```python
result = ('sdktrn'== username)
print(result)
```

    False
    


```python
result = ('sadikturan'== username)
print(result)
```

    True
    


```python
result = (a != b)
print(result)
```

    False
    


```python
result = (a != c)
print(result)
```

    True
    


```python
result = (a > c)
print(result)
```

    False
    


```python
result = (a < c)
print(result)
```

    True
    


```python
result = (a >= b)
print(result)
```

    True
    


```python
result = (c <= b)
print(result)
```

    False
    


```python
result = (True == 1)
print(result)
```

    True
    


```python
result = (False == 0)
print(result)
```

    True
    


```python
result = False + True + 40
print(result)
```

    41
    


```python

```

## QUİZ


```python
# 1- Girilen 2 sayıdan hangisi büyüktür ?

a = int(input("1. Sayı:"))
b = int(input("2. Sayı:"))

result = (a > b)
print(f'a: {a} b: {b} den büyüktür: {result}')
```

    1. Sayı: 2
    2. Sayı: 3
    a: 2 b: 3 den büyüktür: False
    


```python
# 2- Kullanıcıdan 2 vize (%60) ve final (%40) notunu alıp ortalama hesaplayınız.
#    Eğer ortalama 50 ve üstündeyse geçti değilse kaldı yazdırın.

vize1 = float(input('1. vize: '))
vize2 = float(input('2. vize: '))
final = float(input('final : '))

ortalama = (((vize1 + vize2) / 2) * 0.6) + (final * 0.4)

print(f'not ortalamanız : {ortalama} ve dersten geçme durumunuz: {ortalama>=50}')
```

    1. vize:  40
    2. vize:  45
    final :  50
    not ortalamanız : 45.5 ve dersten geçme durumunuz: False
    


```python
# 3- Girilen bir sayının tek mi çift mi olduğunu yazdırın.

sayı = int(input("Sayı Giriniz:"))

tekcift = (sayı % 2 == 0)

print(f"Grimiş olduğunuz Sayınız : {sayı} ve tek-çift durumu {tekcift}")
```

    Sayı Giriniz: 5
    Grimiş olduğunuz Sayınız : 5 ve tek-çift durumu False
    


```python
# 4- Girilen bir sayının negatif pozitif durumunu yazdırın.

sayı = int(input("Sayı Giriniz:"))

pozneg = (sayı>0)

print(f"Grimiş olduğunuz Sayınız : {sayı} ve pozitif mi durumu {pozneg}")
```

    Sayı Giriniz: 8
    Grimiş olduğunuz Sayınız : 8 ve pozitif mi durumu True
    


```python
# 5- Parola ve email bilgisini isteyip doğruluğunu kontrol ediniz.
#    (email: email@sadikturan.com parola:abc123)

dict = {"email": "email@sadikturan.com", "parola" : "abc123"}
email = input("Mailiniz:")
parola = input("Parolanız:")

kontrol1 = (email == dict["email"])
kontrol2 = (parola == dict["parola"])
print(f'Email bilgisi doğrumu: {kontrol1} ve Parola doğru mu: {kontrol2}')
```

    Mailiniz: email@sadikturan.com
    Parolanız: abc123
    Email bilgisi doğrumu: True ve Parola doğru mu: True
    


```python
# 5- Parola ve email bilgisini isteyip doğruluğunu kontrol ediniz.
#    (email: email@sadikturan.com parola:abc123)

email = 'email@sadikturan.com'
password = 'abc123'

girilenEmail = input('email: ')
girilenPassword = input('parola: ')

isEmail = (email == girilenEmail.lower().strip())
isPassword = (password == girilenPassword.lower())

print(f'Email bilgisi doğrumu: {isEmail} ve Parola doğru mu: {isPassword}')
```

## Mantıksal Operatörler


```python
x = 6
hak = 0
devam = 'e'
```


```python
result = 5 < x < 10
print(result) #Bu şekilde yaptığımızda x değerinin 5 ve10 arasında olduğunu belirtir.
```

    True
    


```python
# and operatörü (& bu işareti yapmak için shift + 6 tuşuna basılır)
```


```python
result = (x > 5) and (x < 10) # Her iki şartında sağlanması gerekir.
print(result)
result = (hak > 0) and (devam == 'e') 
print(result)
```

    True
    False
    


```python
# or operatörü (| bu işareti yapmak için ALT GR + < işaretine basılır.)
```


```python
result = (x > 0) or (x % 2 == 0) # Şartlardan bir tanesi sağlanırsa yeterlidir.
print(result)
```

    True
    


```python
# not operatörü
```


```python
result = not(x > 0)
print (result)
```

    False
    


```python
# x, 5-10 arasında olan bir çift sayı mı?

result = (x > 5) and (x < 10) and ( x % 2 == 0)
print (result)
```

    True
    


```python

```

## QUİZ


```python
# 1- Girilen bir sayının 0-100 arasında olup olmadığını kontrol ediniz.

sayı = int(input("Sayı:"))

result = (sayı > 0) and (sayı < 100)
print(f"Girmiş olduğunuz Sayı : {sayı} 0 ile 100 arasında mı? {result}")
```

    Sayı: 34
    Girmiş olduğunuz Sayı : 34 0 ile 100 arasında mı? True
    


```python
# 2- Girilen bir sayının pozitif çift sayı olup olmadığını kontrol ediniz.

sayı = int(input("Sayı:"))

result = (sayı > 0) and (sayı % 2 == 0)
print(f"Girmiş olduğunuz Sayı {sayı} ve hem pozitif hemde çift mi {result}")
```

    Sayı: 12
    Girmiş olduğunuz Sayı 12 ve hem pozitif hemde çift mi True
    


```python
# 3- Email ve parola bilgileri ile giriş kontrolü yapınız. 

email = 'email@sadikturan.com'
password = 'abc123'

g_email = input("Email:")
g_parola = input("Parola:")

result = ( email == g_email) and (password == g_parola)
print(f'uygulamaya giriş başarılı mı: {result}')
```

    Email: 1
    Parola: 2
    uygulamaya giriş başarılı mı: False
    


```python
# 4- Girilen 3 sayıyı büyüklük olarak karşılaştırınız.

a = int(input('a: '))
b = int(input('b: '))
c = int(input('c: '))

result = (a > b) and (a >c)
print(f"a en büyük sayıdır: {result}")

result = (b > a) and (b > c)
print(f'b en büyük sayıdır : {result}')

result = (c > a) and (c > b)
print(f'c en büyük sayıdır : {result}')
```

    a:  1
    b:  2
    c:  3
    a en büyük sayıdır: False
    b en büyük sayıdır : False
    c en büyük sayıdır : True
    


```python
# 5- Kullanıcıdan 2 vize (%60) ve final (%40) notunu alıp ortalama hesaplayınız.
#    Eğer ortalama 50 ve üstündeyse geçti değilse kaldı yazdırın.
#    a-) Ortamalama 50 olsa bile final notu en az 50 olmalıdır.
#    b-) Finalden 70 alındığında ortalamanın önemi olmasın.

vıze1 = int(input("1. Sınavınız:"))
vıze2 = int(input("2. Sınavınız:"))
fınal = int(input("3. Sınavınız:"))

not_hesapla = (((vıze1 + vıze2) / 2) * 0.60) + (fınal * 0.40)

result = (not_hesapla >= 50) or (fınal >=70)
print (f"Aldığınız notun ortalması {not_hesapla} ve dersi geçme durumunuz {result}")

result = (fınal >= 50)
print (f"Aldığınız notun ortalması {not_hesapla} ve dersi geçme durumunuz {result}")

```

    1. Sınavınız: 15
    2. Sınavınız: 15
    3. Sınavınız: 70
    Aldığınız notun ortalması 37.0 ve dersi geçme durumunuz True
    Aldığınız notun ortalması 37.0 ve dersi geçme durumunuz True
    


```python
# 6- Kişinin ad, kilo ve boy bilgilerini alıp kilo indekslerini hesaplayınız.
#    Formül: (Kilo / boy uzunluğunun karesi)
#    Aşağıdaki tabloya göre kişi hangi gruba girmektedir.
#    0-18.4    => Zayıf 
#    18.5-24.9 => Normal  
#    25.0-29.9 => Fazla Kilolu
#    30.0-34.9 => Şişman (Obez)

name = input('adınız: ')
kg = float(input('kilonuz: '))
hg = float(input('boyunuz: '))

index = (kg) / (hg ** 2)
zayif = (index >= 0) and (index<=18.4)
normal = (index>18.4) and (index<=24.9)
kilolu = (index>24.9) and (index<=29.9)
obez = (index>=29.9) and (index<=34.9)

print(f'{name} kilo indeksin: {index} ve kilo değerlendirmen zayıf: {zayif}')
print(f'{name} kilo indeksin: {index} ve kilo değerlendirmen normal: {normal}')
print(f'{name} kilo indeksin: {index} ve kilo değerlendirmen kilolu: {kilolu}')
print(f'{name} kilo indeksin: {index} ve kilo değerlendirmen obez: {obez}')
```

    adınız:  mecit
    kilonuz:  88
    boyunuz:  182
    mecit kilo indeksin: 0.002656683975365294 ve kilo değerlendirmen zayıf: True
    mecit kilo indeksin: 0.002656683975365294 ve kilo değerlendirmen normal: False
    mecit kilo indeksin: 0.002656683975365294 ve kilo değerlendirmen kilolu: False
    mecit kilo indeksin: 0.002656683975365294 ve kilo değerlendirmen obez: False
    


```python

```
