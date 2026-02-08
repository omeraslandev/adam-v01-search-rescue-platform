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

### 🛠️ Donanım Envanteri

| Malzeme | Görev |
| :--- | :--- |
| **ST Nucleo-F411RE** | Ana Kontrol Birimi |
| **MLX90640** | Termal Görüntüleme |
| **VL53L0X** | ToF Lazer Mesafe Sensörü |
| **MPU-6050** | 6 Eksenli İvme ve Gyro |
| **KY-038** | Ses Algılama |
| **3S Lipo Pil** | 11.1V Güç Kaynağı |
