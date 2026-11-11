# 📡 Basit Elektronik Harp Simülasyonu

Greenfoot ortamında geliştirilen, temel radar tespit mekanizmalarını ve elektronik taarruz/koruma (karıştırma ve aldatma) prensiplerini görselleştiren etkileşimli bir simülasyon projesidir.

---

## 👥 Proje Ekibi ve Rol Dağılımı

| Üye | Rol / Görev Alanı | İletişim / GitHub |
| :--- | :--- | :--- |
| **Abdülkadir Aydıngöç** (Takım Lideri) | Simülasyon Mimarisi & Radar Modülü | [@kadir3106](https://github.com/kadir3106) |
| **Turan Kerim** | Greenfoot & Simülasyon Geliştirici | [@turankerim1903-rgb](https://github.com/turankerim1903-rgb) |
| **Proje Üyesi 3** | Greenfoot Senaryo & Arayüz Geliştirme | [@kullanici-adi](https://github.com) |
| **Proje Üyesi 4** | Elektronik Harp (Jammer/Aldatma) Mekanikleri | [@kullanici-adi](https://github.com) |

> *Danışman / Proje Hocası: Atilla Özgür*

---

## 🎯 Projenin Amacı ve Kapsamı
Bu simülasyon, modern radar sistemlerinin çalışma mantığı ile elektronik harp (EH) tekniklerini temel düzeyde görselleştirmeyi amaçlar:

1. **Radar Arama ve Tespit:**
   - 360° döner anten hüzmesi (beam) simülasyonu.
   - Belirli bir menzildeki hedeflerin Radar Kesit Alanı (RCS - Radar Cross Section) mantığıyla tespiti.
2. **Elektronik Taarruz (Karıştırma - Jamming):**
   - Karıştırıcı (Jammer) uçağının radara gürültü yayması (Noise Jamming).
   - Radar ekranında sahte hedefler veya körleme (gürültü hattı) oluşturulması.
3. **Karşı Tedbirler (Chaff / Sahte Hedef):**
   - Radar güdümlü tehditleri yanıltmak için metalize şerit (Chaff) bırakma simülasyonu.

---

## 📁 Proje Dosya Yapısı

\\\	ext
basit-elektronik-harp-simulasyonu/
├── assets/                  # Radar arayüz ikonları, uçak grafikleri, sesler
├── docs/                    # Araştırma raporları, UZEM formları, toplantı notları
│   ├── radar-ve-elektronik-harp-arastirmasi.md
│   └── uzem-2-haftalik-rapor-taslagi.md
├── src/                     # Greenfoot Java senaryo kodları (World, Radar, Target, Jammer)
├── .gitignore               # Java ve Greenfoot derleme filtreleri
└── README.md                # Ana proje dökümantasyonu
\\\

---

## 🤝 4 Kişilik Takım İçin Git Kuralları (Önemli!)

Çakışma (conflict) yaşamamak ve düzenli çalışmak için ekip şu adımları izler:

1. **Doğrudan main dalına commit atılmaz.**
2. Her yeni özellik için kendi dalınızı açın:
   - \git checkout -b feat/radar-tespit\
   - \git checkout -b feat/jammer-mekanigi\
3. Çalışmaya başlamadan önce her zaman en güncel kodu çekin:
   - \git pull origin main\
4. İşinizi bitirince GitHub üzerinden **Pull Request (PR)** açın, en az bir ekip arkadaşınız inceleyip onaylasın.
5. Commit mesajları anlaşılır olmalıdır (örn: eat: radar tarama acisi eklendi).

---

## 🚀 Başlarken
1. Depoyu klonlayın:
   \\\ash
   git clone https://github.com/kadir3106/basit-elektronik-harp-simulasyonu.git
   \\\
2. Greenfoot uygulamasını açın -> **Scenario** -> **Open** seçeneğinden src klasörünü yükleyin.


