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
