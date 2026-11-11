# 📡 Radar ve Elektronik Harp (EH) Ön Araştırma Raporu

**Hazırlayan:** Abdülkadir Aydıngöç & Proje Ekibi  
**Tarih:** Kasım 2026  
**Danışman:** Atilla Özgür  

---

## 1. Radar Nedir ve Nasıl Çalışır?
**RADAR** (*Radio Detection and Ranging*), radyo dalgaları kullanarak uzaktaki nesnelerin (uçak, gemi, araç vb.) varlığını, yönünü, mesafesini ve hızını tespit eden bir sistemdir.

### Temel Çalışma Prensibi:
1. **Darbe İletimi (Transmitter):** Radar anteni yüksek frekanslı bir radyo darbesi (pulse) yayar.
2. **Yansıma (Echo):** Yayılan dalga bir hedefe (örn. uçak) çarptığında bir kısmı geri yansır.
3. **Mesafe Hesabı:** Sinyalin gidip gelme süresi ($\Delta t$) ve ışık hızı ($) kullanılarak hedefin menzili ($) hesaplanır:
   R = \frac{c \cdot \Delta t}{2}
4. **Hedef Tespiti:** Yansıyan sinyalin gücü hedefin **Radar Kesit Alanı**na (RCS - *Radar Cross Section*) bağlıdır.

---

## 2. Elektronik Harp (Electronic Warfare - EW)
Elektronik Harp, elektromanyetik tayfın (spektrumun) kontrolünü sağlamak amacıyla dost unsurların radar/telsiz haberleşmesini korurken düşmanınkini etkisiz hale getirme sanatıdır.

Elektronik Harp üç ana disipline ayrılır:
1. **Elektronik Taarruz (EA - Electronic Attack / ECM):** Düşman radarlarını karıştırma veya aldatma.
2. **Elektronik Koruma (EP - Electronic Protection / ECCM):** Kendi radarlarımızı düşman karıştırmasından koruma tedbirleri.
3. **Elektronik Destek (ES - Electronic Warfare Support / ESM):** Düşman radar sinyallerini dinleme, tespit ve analiz etme.

---

## 3. Simülasyonumuzda Yer Alacak Temel Mekanikler
Geliştireceğimiz Greenfoot simülasyonunda modellenmesi hedeflenen senaryolar:

### A. Gürültü Karıştırması (Noise Jamming - Körleme)
- Karıştırıcı (Jammer) uçağı radara doğru yüksek güçlü sürekli gürültü sinyali gönderir.
- Radar ekranında o yönde geniş bir parlak kama (strobe) oluşur ve radar arkasındaki hedefleri göremez.

### B. Aldatma Karıştırması (Deception Jamming)
- Karıştırıcı gelen radar sinyalini alır, çok az geciktirip geri yansıtır.
- Radar ekranında gerçekte olmayan **sahte hedefler (ghost targets)** belirir.

### C. Chaff (Metalize Şerit Bulutu)
- Uçak, radar dalgalarını yoğun şekilde yansıtan alüminyum/cam elyaf şeritler bırakır.
- Radar güdümlü füzeler veya radar operatörü asıl uçak yerine devasa bir bulut ekosu görür.

---

## 4. Ekip İçi Radar Uzmanı Seçimi
Hocamızın belirttiği üzere gruptan bir kişi **Radar Uzmanı** olarak seçilecek ve radar denklemleri, anten yayılım diyagramları ve frekans bantları üzerinde derinleşecektir.

---

## 5. İncelenen Kaynaklar ve İlgili Bölümler (Kaynakça)

> *Not: Proje başlangıç aşamasında kitapların ve makalelerin tamamı yerine, simülasyonumuzda doğrudan modelleyeceğimiz matematiksel denklemler ve temel konseptleri içeren spesifik bölümler incelenmiştir.*

### 📚 1. Kitap Kaynağı (Radar Temelleri):
* **Eser:** Merrill I. Skolnik – *Introduction to Radar Systems* (McGraw-Hill)
* **İncelenen Bölüm:** **Chapter 1: An Introduction to Radar**
  * *Bölüm 1.1:* Radar Principle (Radar Çalışma İlkesi) — Sayfa 1–6
  * *Bölüm 1.2:* The Simple Form of the Radar Equation (Basit Radar Menzil Denklemi) — Sayfa 6–11
* **Projeye Katkısı:** Simülasyondaki radar kulesinin hedefi tespit etme mesafesi ($) ve sinyal gidiş-dönüş süresi hesaplamaları bu bölüme dayandırılmıştır.

### 📚 2. Kitap Kaynağı (Elektronik Harp & Karıştırma):
* **Eser:** David L. Adamy – *EW 101: A First Course in Electronic Warfare* (Artech House)
* **İncelenen Bölüm:** **Chapter 4: Electronic Attack & Jamming Techniques**
  * *Alt Başlık:* Noise Jamming and Power Consideration (Gürültü Karıştırması ve Güç Oranı) — Sayfa 85–98
  * *Alt Başlık:* Chaff and Decoys (Yanıltıcı Şeritler ve Sahte Hedefler) — Sayfa 115–122
* **Projeye Katkısı:** Uçağın jammer açtığında radara basacağı gürültü seviyesi (J/S - Jammer-to-Signal oranı) ve radar ekranındaki körleme kama açısının mantığı bu kısımdan alınmıştır.

### 🌐 3. Açık Kaynak Teknik Eğitim Portalı:
* **Kaynak:** Christian Wolff – *Radartutorial.eu* (Uluslararası Açık Radar Eğitim Platformu)
* **İncelenen Modül:** 
  * *Radar Basics:* Plan Position Indicator (PPI Ekranı - 360° Dönen Ekran Mantığı)
  * *Electronic Countermeasures (ECM):* Noise Strobe & Jamming Effects on PPI Displays
* **Projeye Katkısı:** Greenfoot üzerinde 2 boyutlu döner anten ve ekrandaki hedef izlerinin (blip) görselleştirilmesinde referans alınmıştır.

### 📄 4. Türkçe Teknik İnceleme:
* **Kaynak:** Savunma Sanayii Dergisi / Teknik Blog Yayınları
* **İncelenen Konu:** *Elektronik Harp Sistemlerinde Karıştırma ve Aldatma Tekniklerinin Sınıflandırılması*
* **Projeye Katkısı:** Terimlerin Türkçe akademik karşılıkları (Elektronik Taarruz, Gürültü Karıştırması vb.) UZEM raporlarına uygun hale getirilmiştir.
