# A.D.A.M. v0.1 (Altyapıdan Bağımsız Dağıtık Arama Modülleri) 🤖

[cite_start]**A.D.A.M. v0.1**, kritik altyapıların (GSM, GPS, İnternet) çöktüğü afet bölgelerinde arama-kurtarma operasyonları için "ileri göz" olarak tasarlanmış, düşük maliyetli bir mobil robotik sensör platformudur[cite: 569, 571, 580]. [cite_start]Bu proje, tehlikeli ortamlarda canlı tespiti için sağlam bir kavram kanıtı (PoC) oluşturmayı amaçlayan "Asker" mobil birimlerinin ilk donanım versiyonudur[cite: 571, 572, 574].

---

### ⚠️ Proje Durumu

| Parametre | Mevcut Durum |
| :--- | :--- |
| **Program** | [cite_start]TÜBİTAK 2209-A Üniversite Öğrencileri Araştırma Projeleri Destekleme Programı [cite: 567, 619] |
| **Aşama** | [cite_start]Başvuru Değerlendirme Süreci  |
| **Destek Durumu** | Henüz resmi bir destek/fon almamıştır; tüm süreçler konsept aşamasındadır. |

---

### 🌟 Temel Özellikler ve Sensör Füzyonu

[cite_start]Enkaz altındaki yaşam belirtilerini tespit etmek için kullanılan sensör mimarisi aşağıdadır[cite: 573, 584]:

| Sensör | İşlev | Teknik Detay |
| :--- | :--- | :--- |
| **Termal Kamera** | Canlı Tespiti | [cite_start]MLX90640 ile ısı imzası ve hotspot tespiti[cite: 573, 593]. |
| **Mikrofon** | Ses Tespiti | [cite_start]Yardım çığlıklarını veya yapısal sesleri yakalama[cite: 573, 596]. |
| **ToF Lazer** | Uzamsal Farkındalık | [cite_start]VL53L0X ile çarpışma önleme ve mesafe ölçümü[cite: 573, 594]. |
| **IMU** | Stabilite | [cite_start]MPU-6050 ile robotun denge ve yönelim takibi[cite: 573, 595]. |

---

### 🛠️ Donanım Envanteri

| Malzeme | Görev |
| :--- | :--- |
| **ST Nucleo-F411RE** | [cite_start]Ana Kontrol Birimi [cite: 589, 642] |
| **MLX90640** | [cite_start]Termal Görüntüleme [cite: 593, 643] |
| **VL53L0X** | [cite_start]ToF Lazer Mesafe Sensörü [cite: 594, 650] |
| **MPU-6050** | [cite_start]6 Eksenli İvme ve Gyro [cite: 595, 651] |
| **KY-038** | [cite_start]Ses Algılama [cite: 596, 652] |
| **3S Lipo Pil** | [cite_start]11.1V Güç Kaynağı [cite: 597, 644] |
