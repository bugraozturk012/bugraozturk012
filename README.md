<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/bugraozturk012/bugraozturk012/main/varlik/banner-koyu.svg">
  <img alt="Buğra Öztürk — Otonom Sistemler, Yapay Görü, Web ve Mobil" src="https://raw.githubusercontent.com/bugraozturk012/bugraozturk012/main/varlik/banner-acik.svg">
</picture>

Manisa Celal Bayar Üniversitesi Bilgisayar Mühendisliği 3. sınıf öğrencisiyim.
İlgi alanım bir sistemin **uçtan uca** çalışması: sensörden gelen veriden
karar veren yazılıma, oradan da onu kullanan kişinin gördüğü arayüze kadar.

TEKNOFEST'te iki takımı yönetiyorum: bir otonom kara aracı ve bir havadan görüntü
analizi takımı. Bunların yanında üniversitenin Proje Koordinasyon ve Araştırma
Merkezi'nde web geliştirici olarak çalışıyorum.

---

## Üzerinde çalıştıklarım

### 🚙 LYDİA — Otonom Kara Aracı · TEKNOFEST 2026 İKA **finalisti**
**MCBÜ MAGNESİA** · Takım Kaptanı, Otonom Yazılım
→ **[`teknofest_ika`](https://github.com/bugraozturk012/teknofest_ika)**

Ackermann direksiyonlu aracın Jetson Orin Nano üzerinde koşan **ROS 2 otonom
yığınını** kurdum. Nav2'yi araç kinematiğine ve gövde ölçülerine göre
yapılandırdım. Yığının hiç ayağa kalkmamasına yol açan davranış ağacını yeniden
yazdım. EKF ile tekerlek ve IMU verisini birleştiren konumlamayı ve SMACH tabanlı
görev yöneticisini yazdım. Haritaya ihtiyaç duymayan bir **kayan hedef** sistemi
geliştirdim: hedefi aracın o anki LiDAR taramasından üretiyor ve parkurun CAD
çiziminden alınan sanal taramalarla doğrulandı. YOLOv8 tespitlerini LiDAR ile
eşleştiren füzyon hattını ve sahada kullanılan telemetri panosunu da ben kurdum.

Karar mantığını ROS'tan bağımsız saf fonksiyonlarda topladım. Böylece araç
olmadan da test edilebiliyor: **1000'i aşkın birim testi** var ve kritik
kapılar mutasyon testiyle sınanıyor.

### 🛩️ Havacılıkta Yapay Zekâ · TEKNOFEST 2026
Takım Lideri · 2 kişilik ekip
→ **[`teknofest_havacilikta_yapayzeka`](https://github.com/bugraozturk012/teknofest_havacilikta_yapayzeka)**

Drone görüntülerinde gerçek zamanlı **nesne tespiti** ve GPS devre dışıyken
**görsel konum kestirimi**. Taşıt ve insan tespiti için YOLOv8s ile ByteTrack
kullandım. Konum kestiriminde optik akış, RANSAC homografi ve Kalman
filtresini birlikte çalıştırdım. Görüntü eşleştirmede DINOv2 ve SIFT aynı karede
paralel koşuyor, birinin kaçırdığını öteki yakalıyor. Takım lideri olarak görev dağılımını ve yarışma takvimini
de yürüttüm.

### 📱 Ehliyet Soru Çözümleri 2026 · MotiveX Intelligence stajı
Flutter ile geliştirilen ve App Store'da yayında olan e-sınav hazırlık
uygulaması. Tutarlı bir tasarım sistemi kurdum ve istatistik ekranını sıfırdan
yazdım. Soru havuzunu yaklaşık 60 Python denetim betiğiyle taradım:
**3435 → 2062 soru**, cevabı uzunluğundan belli olan **153 soru → 0**.

### 🐔 Kümes İzleme Robotu · TÜBİTAK 1711
Broiler kümeslerinde dolaşıp hayvanları izleyen otonom robot. Raspberry Pi 5,
ESP32 ve Hailo-8L'den oluşan donanımı seçtim. Üç katmanlı tespite dayanan
davranış mimarisini tasarladım.

---

## Kullandıklarım

```
robotik      ROS 2 Humble · Nav2 · SLAM Toolbox · robot_localization (EKF)
             SMACH · Ackermann kinematiği · Jetson Orin Nano · Raspberry Pi 5
yapay görü   YOLOv8 · ByteTrack · OpenCV · PyTorch · DINOv2 · TensorRT
             optik akış · Kalman filtresi · LiDAR–kamera füzyonu
gömülü       STM32 · ESP32 · Arduino · UART seri protokol · Hailo-8L
web          React · Next.js · TypeScript · Tailwind CSS · Node.js · HTML/CSS
mobil        Flutter · Dart · Riverpod · SQLite · Firebase
araçlar      Linux · WSL2 · systemd · Git & GitHub · pytest · Figma
dil          Python · C · C++ · JavaScript / TypeScript · Dart · SQL
```

## Nasıl çalışırım

**Önce ölç, sonra karar ver.** Sahada gördüğüm bir arızayı koddan tahmin etmek
yerine log'dan, ölçümden ya da koşturarak doğrularım. Emin olamadığım bir şeyi
emin olmadığımı söyleyerek yazarım.

**Test, davranışı kilitlemeli.** Bir testin işe yaradığını, test ettiği kodu
bilerek bozup testin kırıldığını görünce kabul ederim.

**Arıza durumu da tasarımın parçası.** Bir sensör sustuğunda ya da bağlantı
koptuğunda sistemin ne yapacağını baştan yazarım. Arayüzde de aynısı geçerli:
yükleniyor, hata ve boş durumları ilk günden tasarlanır.

**İncelenebilir teslim.** Büyük değişiklikleri, her biri tek başına anlaşılan
küçük commit'lere bölerim.

## İletişim

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bu%C4%9Fra-%C3%B6zt%C3%BCrk-67a573293/)
[![E-posta](https://img.shields.io/badge/E--posta-24292F?style=flat-square&logo=gmail&logoColor=white)](mailto:ozturkbugra684@gmail.com)
