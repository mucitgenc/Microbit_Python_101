# Mucit Genç - Python 101 Eğitimi / Ders 2



##  Ekran İşlemleri @unplugged 

Pixel nedir?


##  Programlama Dili  

Görüntüyü oluşturan her bir noktacığa pixel denir. <br>
Bir pixelin renk aralığı ne kadar fazla ise o pixel de renk havuzunda gerçeğe daha yakın bir renk verecektir. <br>
Buna renk derinliği denir. Genelde "bit " olarak ifade edilir. 1 bit renk derinliğine sahip bir noktacık 2 adet renk alabilir.<br>
1 bit renk derinliğine sahip bir noktacık 21 = 2 adet renk alabilir. (siyah ve beyaz)<br>
2 bit renk derinliğine sahip bir noktacık 22 = 4 adet renk alabilir.<br>
RGB, monitör ve televizyonlarda kullanılan renk uzayıdır.<br>
Kanal başına 8 bit renk derinliği seçersek her kanalda da 256 farklı renk tonu ifade edebiliriz.<br>

``||Basic:Piksel Nedir?||``

```python
basic.show_leds("""
0 0 0 0 0
0 0 0 0 0
0 0 1 0 0
0 0 0 0 0
0 0 0 0 0
""")
```

**Piksel Nedir?**
![Aritmetik Operatörler](https://lh4.googleusercontent.com/sBR8eEFgD1Bt3_n0ik01SmNZ_0IwgqtYWcLT42_THRoHgkgpg8i0Y7jP-ZGRnSN70G8gPeAr4b-oieXKe_IB=w1919-h887)


##  Animasyon Nedir? @unplugged 

Animasyon Nedir?

## Animasyon @fullscreen

Animasyon (canlandırma), birkaç resmin arka arkaya hızlı bir şekilde gösterilmesiyle elde edilen hareketli görüntüdür.<br>
İlk animasyonlar birkaç kağıda istenen resimlerin çizilmesi ve kâğıtların hızlıca geçirilmesi veya bir çemberin içine konup döndürülmesi ile yapılıyordu.<br>


``||Basic:Kalp Animasyonu||``

```python
basic.show_leds("""
    0 1 0 1 0
    1 1 1 1 1
    1 1 1 1 1
    0 1 1 1 0
    0 0 1 0 0
    """)
basic.show_leds("""
    0 0 0 0 0
    0 1 0 1 0
    0 1 1 1 0
    0 1 1 1 0
    0 0 1 0 0
    """)
```
En az 14.000 yaşında
![Aritmetik Operatörler](https://lh4.googleusercontent.com/8LvZHV3hEv6Gav7p0fuK2TIOACFMfYxtad-J76IrO05j5Vsyl2G8FaPunT2Qg8eFfCWxOWKw0JYM86UChfmz=w1919-h887)

## Bekleme Fonksyonu @fullscreen

Söylediğiniz milisaniye boyunca programı bekletin. Programınızı bekletmek için bu işlevi kullanabilirsiniz.

``||Basic:basic.pause(100)||``

```python
basic.show_icon(IconNames.HEART)
basic.pause(1000)
basic.show_icon(IconNames.SMALL_HEART)
basic.pause(1000)
```

## Sürekli Tekrarla Fonksyonu @fullscreen

Döngünün içerisinde yazılan programın bir parçasını arka planda çalıştırmaya devam eder .

``||Basic:run code forever||``

```python
def on_forever():
    basic.show_icon(IconNames.HEART)
    basic.pause(1000)
    basic.show_icon(IconNames.SMALL_HEART)
    basic.pause(1000)
basic.forever(on_forever)
```


## Metinsel değişken tipi(string) @fullscreen

Python'daki Metinsel Değişkenler tek tırnak işareti veya çift tırnak işareti ile çevrilidir.
**'merhaba', "merhaba" ile aynıdır.**

Python 3 kodlarında print() fonksyonu ile bir metinsel değişkenin değerini görüntüleyebilirsiniz

Microbitin LED ekranda bir metinsel değişkeni göstermek için ise basic.show_string() foksyonu kullanılır. 
Ekrandan daha büyükse sola kayar.

``||Basic:basic.show_string()||``

```python
basic.show_string("Merhaba Dünya")
```

## Sayısal değişken tipi(number) @fullscreen

Python'da değişkenlere sayılar atanırken doğrudan atama işlemi yapılır.Herhangi bir tırnak işareti kullanılmaz.

Python'da üç sayısal tür vardır:
**int**  tamsayılar
**float** Ondalıklı sayılar
**complex** karmaşık sayılar

Python 3 kodlarında print() fonksyonu ile bir sayısal değişkenin değerini görüntüleyebilirsiniz

Microbitin LED ekranda bir sayısal değişkeni göstermek için ise basic.show_number() foksyonu kullanılır. 
Ekrandan daha büyükse sola kayar.

``||Basic:basic.show_number()||``

```python
basic.show_number(1453)
```
## Alıştırma Zamanı @fullscreen

**Ekranda sürekli olarak Adını 5sn Yaşını 3sn yazan bir program yazabilirmisin?**


```python
def on_forever():
    basic.show_string("Ad")
    basic.show_number("yaş")
basic.forever(on_forever)
```


## Alıştırma Zamanı @fullscreen

**Günlük Hayatta kullandığımız Trafik Lambalarının Çalışma Algoritmasını yazabilir misin?**<br>
50sn Yeşil="Y"<br>
15sn Sarı="S"<br>
30sn Kırmızı="K"<br>

## Mucit Genç Bilgilendirme! @unplugged  

![Algoritmalar Hayatımızın Neresinde ?](/static/mb/projects/a4-motion.png)

**Algoritmalar Heyerde?**

1. Trafikte
2. Alışverişte
3. Sosyal Medyada
4. Not hesaplamalarında
5. Projelerde
6. Mimari yapılarda
7. Hastanede
8. Pizza Siparişinde
9. instagram önerilerinde
10. Bu yazıda