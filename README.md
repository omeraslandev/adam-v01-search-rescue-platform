# A.D.A.M. v0.1 (Altyapıdan Bağımsız Dağıtık Arama Modülleri) 🤖

**A.D.A.M. v0.1**, kritik altyapıların (GSM, GPS, İnternet) çöktüğü afet bölgelerinde arama-kurtarma operasyonları için "ileri göz" olarak tasarlanmış, düşük maliyetli bir mobil robotik sensör platformudur. Bu proje, tehlikeli ortamlarda canlı tespiti için sağlam bir kavram kanıtı (PoC) oluşturmayı amaçlayan "Asker" mobil birimlerinin ilk donanım versiyonudur.

---

### ⚠️ Proje Durumu

| Parametre | Mevcut Durum |
| :--- | :--- |
| **Program** | TÜBİTAK 2209-A Üniversite Öğrencileri Araştırma Projeleri Destekleme Programı |
| **Aşama** | Başvuru Değerlendirme Süreci |
| **Destek Durumu** | Henüz resmi bir destek/fon almamıştır; tüm süreçler konsept aşamasındadır. |

---

### 🌟 Temel Özellikler ve Sensör Füzyonu

Enkaz altındaki yaşam belirtilerini tespit etmek için kullanılan sensör mimarisi aşağıdadır:

| Sensör | İşlev | Teknik Detay |
| :--- | :--- | :--- |
| **Termal Kamera** | Canlı Tespiti | MLX90640 ile ısı imzası ve hotspot tespiti. |
| **Mikrofon** | Ses Tespiti | Yardım çığlıklarını veya yapısal sesleri yakalama. |
| **ToF Lazer** | Uzamsal Farkındalık | VL53L0X ile çarpışma önleme ve mesafe ölçümü. |
| **IMU** | Stabilite | MPU-6050 ile robotun denge ve yönelim takibi. |

---

### 🎯 Başarı Kriteri: "Kör Operatör" Test Senaryosu

Platformun başarısı, operatörün robotu fiziksel olarak görmeden, sadece sensör verilerini kullanarak görevini tamamlamasıyla ölçülür:

* **Senaryo:** Robot, operatörün görüş alanı dışındaki bir engel parkuruna yerleştirilir. 
* **Navigasyon:** Operatör, sadece ToF mesafe verilerine bakarak robotu engellere çarpmadan yönlendirir.
* **Tespit:** Parkur sonundaki gizli ısı kaynağı (Termal) ve ses kaynağı (Mikrofon) başarıyla tespit edilip komuta merkezine raporlandığında test başarılı sayılır.

---

### 🗺️ Gelecek Yol Haritası

| Sürüm | Temel Hedef | Teknoloji Odağı |
| :--- | :--- | :--- |
| **v1.0 - v2.0** | Kablosuz İletişim | Kendi kendini onaran LoRa Mesh ağ yapısı. |
| **v3.0** | Otonom Sürü Zekası | Sürü robotu algoritmaları ve engelden otonom kaçınma. |
| **v4.0** | Gelişmiş Mobilite | Dinamik enkaz tırmanma kabiliyetine sahip şasi güncellemeleri. |

---

### 🛠️ Donanım Envanteri

| Malzeme | Görev |
| :--- | :--- |
| **ST Nucleo-F411RE** | Ana Kontrol Birimi (İşlemci) |
| **MLX90640** | Termal Görüntüleme Sensörü |
| **VL53L0X** | ToF Lazer Mesafe Sensörü |
| **MPU-6050** | 6 Eksenli İvme ve Gyro (IMU) |
| **KY-038** | Ses Algılama Sensörü (Mikrofon) |
| **3S Lipo Pil** | 11.1V Sistem Güç Kaynağı |

---

### 🛡️ Etik ve Güvenlik Standartları

* **İş Güvenliği:** Üretim sürecinde lehimleme işlemleri sırasında koruyucu gözlük ve eldiven kullanılır; çalışma alanı aktif olarak havalandırılır.
* **Toplumsal Fayda:** Proje, AFAD ve itfaiye gibi ekiplerin hayatını riske atmadan "altın saatler" içinde veri toplamasını amaçlayan "önce insan" felsefesiyle geliştirilmektedir.
* **Veri Etiği:** Toplanan sensör verileri sadece hayat kurtarma amacıyla kullanılır ve otonom sistemlerde etik karar alma sınırlarına sadık kalınır.
