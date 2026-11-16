# Radar ve Elektronik Harp Ön Araştırma Notları

**Proje:** Basit Elektronik Harp Simülasyonu  
**Proje Danışmanı:** Dr. Öğr. Üy. Atilla Özgür  
**Hazırlayanlar:** M. Emin Çetin (Radar Uzmanı), Abdülkadir Aydıngöç, Turan Kerim, Burak Arı  

---

## 1. GİRİŞ

a. Bu çalışma, Greenfoot ortamında geliştireceğimiz Basit Elektronik Harp Simülasyonu projesi öncesinde radar çalışma prensiplerini ve temel karıştırma (jamming) yöntemlerini incelemek amacıyla hazırlanmıştır.

b. Simülasyonda temel olarak bir arama radarının 360 derece tarama yapması, menzile giren hedefleri tespit etmesi ve elektronik taarruz uygulayan unsurların radarı yanıltması modellenecektir.

---

## 2. İNCELEME

### a. Radar Çalışma Prensibi

(1) RADAR (*Radio Detection and Ranging*), radyo dalgaları yardımıyla hedeflerin mesafesini, yönünü (açısını) ve hızını tespit eden sistemdir (Skolnik, 2001:1-6).

(2) Temel tespit süreci şu adımlarla gerçekleşir:

(a) Anten belirli bir yönde elektromanyetik sinyal darbesi gönderir.

(b) Sinyal hedefe çarpar ve bir kısmı antene geri yansır. Yansıyan sinyalin büyüklüğü hedefin Radar Kesit Alanı (RKA) değerine bağlıdır (Skolnik, 2001:8).

(c) Sinyalin gidip gelme süresi ($\Delta t$) ve ışık hızı ($c$) üzerinden hedefin mesafesi ($R$) hesaplanır (Skolnik, 2001:3):

$$R = \frac{c \cdot \Delta t}{2}$$

### b. Elektronik Harp (EH) ve Alt Başlıkları

(1) Elektronik Harp (EH), elektromanyetik spektrumdan dost unsurların yararlanmasını sağlarken düşman kullanımını engellemek veya zorlaştırmak için yapılan faaliyetlerdir (Adamy, 2001:1-4). Üç ana başlığa ayrılır:

(a) **Elektronik Taarruz (ET):** Düşman radar ve haberleşme sistemlerini karıştırma veya aldatma faaliyetleri (Adamy, 2001:85).

(b) **Elektronik Koruma (EK):** Kendi radar sistemlerimizi düşman karıştırmasına karşı koruma tedbirleri.

(c) **Elektronik Destek (ED):** Düşman yayınlarını dinleme ve tespit etme faaliyetleri.

### c. Simülasyonda Uygulanacak Karıştırma Yöntemleri

(1) **Gürültü Karıştırması (Noise Jamming):** Karıştırıcı uçağın radara yüksek güçlü gürültü sinyali göndermesidir. Karıştırma gücü hedef yansımasından yüksek olduğunda (J/S oranı), radar ekranında o açı boyunca parlak bir gürültü çizgisi oluşur ve radar o bölgedeki hedefleri göremez (Adamy, 2001:88-95; Wolff, 2024).

(2) **Aldatma Karıştırması (Deception Jamming):** Radardan gelen sinyalin geciktirilerek geri gönderilmesiyle radar ekranında sahte hedefler oluşturulmasıdır (Adamy, 2001:96-98).

(3) **Chaff (Metalize Şerit):** Uçaktan bırakılan ince metal şeritlerin radar dalgalarını yansıtarak ekranda yanıltıcı bir bulut oluşturmasıdır (Adamy, 2001:115-122).

---

## 3. SONUÇ

a. Yapılan inceleme sonucunda radar tarama ekranının, hedef tespitinin ve gürültü karıştırması (körleme) mekaniğinin Greenfoot üzerinde `World`, `Radar`, `Target` ve `Jammer` sınıfları ile simüle edilebileceği değerlendirilmiştir.

b. Takım içinde **M. Emin Çetin** radar uzmanı olarak belirlenmiş olup, menzil ve karıştırma hesaplamaları kendisi tarafından koordine edilecektir.

---

## KAYNAKLAR

Adamy, D., (2001), <u>EW 101: A First Course in Electronic Warfare</u>, Artech House, Boston, 1. Baskı, ss: 85-122.

Skolnik, M., (2001), <u>Introduction to Radar Systems</u>, McGraw-Hill, New York, 3. Baskı, ss: 1-11.

Wolff, C., (2024), "Radar Basics & Electronic Countermeasures (ECM)", <u>Radartutorial.eu</u>, https://www.radartutorial.eu (Erişim: 11.11.2026).
