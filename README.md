# A.D.A.M. v0.1 (Altyapıdan Bağımsız Dağıtık Arama Modülleri) 🤖

**A.D.A.M. v0.1**, kritik altyapıların (GSM, GPS, İnternet) çöktüğü afet bölgelerinde arama-kurtarma operasyonları için "ileri göz" olarak tasarlanmış, düşük maliyetli bir mobil robotik sensör platformudur. Bu proje, tehlikeli ortamlarda canlı tespiti için sağlam bir kavram kanıtı (PoC) oluşturmayı amaçlayan "Asker" mobil birimlerinin ilk donanım versiyonudur.

---

### ⚠️ Proje Durumu

| Parametre | Mevcut Durum |
| --- | --- |
| **Program** | TÜBİTAK 2209-A Üniversite Öğrencileri Araştırma Projeleri Destekleme Programı 

 |
| **Aşama** | Başvuru Değerlendirme Süreci 

 |
| **Destek Durumu** | Henüz resmi bir destek/fon almamıştır; tüm süreçler konsept aşamasındadır. |

---

### 🌟 Temel Özellikler ve Sensör Füzyonu

Enkaz altındaki yaşam belirtilerini tespit etmek için kullanılan sensör mimarisi aşağıdadır:

| Sensör | İşlev | Teknik Detay |
| --- | --- | --- |
| **Termal Kamera** | Canlı Tespiti | MLX90640 ile ısı imzası ve hotspot tespiti.

 |
| **Mikrofon** | Ses Tespiti | Yardım çığlıklarını veya yapısal sesleri yakalama.

 |
| **ToF Lazer** | Uzamsal Farkındalık | VL53L0X ile çarpışma önleme ve mesafe ölçümü.

 |
| **IMU** | Stabilite | MPU-6050 ile robotun denge ve yönelim takibi.

 |

---

### 🏗️ Sistem Mimarisi (v0.1)

Bu versiyon, radyo frekanslarının riskli olduğu bölgelerde güvenilir veri akışı için kablolu bir yapıya odaklanır:

| Bileşen | Detay |
| --- | --- |
| **Ana İşlemci** | STM32 Geliştirme Kartı (Gömülü C/C++ ile programlanmıştır).

 |
| **Hareket Sistemi** | Enkaz üzerinde manevra kabiliyeti için paletli robot şasisi.

 |
| **Bağlantı** | Komuta Merkezi terminaline USB-UART üzerinden kablolu seri iletişim.

 |
| **Arayüz** | Isı, mesafe ve ses seviyelerinin gerçek zamanlı izlendiği terminal.

 |

---

### 🎯 Başarı Kriteri: "Kör Operatör" Testi

Platformun başarısı, operatörün robotu fiziksel olarak görmeden, sadece sensör verilerini kullanarak engelli bir parkuru tamamlamasıyla ölçülür:

* 
**Görev**: Sensör verilerine bakarak engellere çarpmadan ilerleme.


* 
**Hedef**: Parkur sonundaki ısı ve ses kaynağının başarıyla raporlanması.



---

### 🗺️ Gelecek Yol Haritası

| Sürüm | Temel Hedef | Teknoloji |
| --- | --- | --- |
| **v1.0 - v2.0** | Kablosuz İletişim | Kendi kendini onaran LoRa Mesh ağ yapısı.

 |
| **v3.0** | Otonom Sürü | Gelişmiş sürü zekası algoritmaları.

 |

---

### 🛠️ Donanım Envanteri

| Malzeme | Görev |
| --- | --- |
| **ST Nucleo-F411RE** | Ana Kontrol Birimi 

 |
| **MLX90640** | Termal Görüntüleme 

 |
| **VL53L0X** | ToF Lazer Mesafe Sensörü 

 |
| **MPU-6050** | 6 Eksenli İvme ve Gyro 

 |
| **KY-038** | Ses Algılama 

 |
| **3S Lipo Pil** | 11.1V Güç Kaynağı 

 |

---

### 🛡️ Etik ve Güvenlik Standartları

* Lehimleme işlemleri sırasında koruyucu gözlük, eldiven ve uygun havalandırma kullanımı esastır.


* Proje, ilk müdahalecilerin (AFAD, itfaiye vb.) hayatını riske atmadan veri toplamasını amaçlayan "önce insan" felsefesiyle tasarlanmıştır.
