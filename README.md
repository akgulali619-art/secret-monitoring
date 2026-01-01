⚠️ YASAL UYARI (DISCLAIMER)

Bu araç SADECE eğitim, siber güvenlik farkındalığı ve laboratuvar çalışmaları amacıyla paylaşılmıştır.
Bu kodun izinsiz veya etik dışı kullanımı yasal sorumluluk doğurabilir.
Geliştirici, aracın kötüye kullanımından doğacak hiçbir zarardan sorumlu tutulamaz.

Bu uygulama yalnızca kendi cihazlarınızda veya açık izin aldığınız test ortamlarında kullanılmalıdır.
Uygulama internet ortamına (Cloudflare, Ngrok vb.) açıldıysa, test tamamlandıktan sonra erişim kapatılmalıdır.

🚀 Kullanım ve Kurulum Rehberi (Canlı Erişim)

Bu aracı yerel ağınızda veya bir test sunucusunda çalıştırmak için aşağıdaki adımları takip edebilirsiniz.

1. Hazırlık ve Kurulum

Bilgisayarınızda Python 3.x yüklü olduğundan emin olun.

git clone https://github.com/kullaniciadin/pip-analiz-poc.git
cd pip-analiz-poc
pip install flask flask-socketio

2. Sunucuyu Başlatma
python app.py


Sunucu çalıştığında uygulamaya aşağıdaki adreslerden erişebilirsiniz:

Yerel: http://localhost:5000

Test tüneli (Cloudflare / Ngrok vb.)

3. Uygulama ve Test (Adım Adım)

Bu test, kendi cihazınızda veya izinli bir test cihazında yapılmalıdır.

Test cihazında (Android önerilir) tarayıcıyı açın ve sunucu adresine gidin.

“Analizi Başlat” butonuna tıklayın.

Tarayıcı kamera izni istediğinde bilinçli olarak izin verin.

Kamera açıldıktan sonra ana ekrana döndüğünüzde Picture-in-Picture (PiP) modu aktif olabilir.

Panel üzerinden görüntü akışının devam ettiğini gözlemleyin.

Bu davranış, modern tarayıcıların medya yönetim sınırlarını test etmek amacıyla kullanılmaktadır.

4. Platform Farklılıkları

Android: PiP modu sayesinde kamera akışı arka planda devam edebilir.

iOS / iPadOS: Apple güvenlik politikaları gereği uygulama arka plana alındığında kamera otomatik olarak durdurulur.

🛠️ Kurulum ve Kullanım Kılavuzu (Video Kayıt Destekli)

Bu proje, PiP API ve MediaStream gibi web teknolojilerinin güvenlik sınırlarını incelemek için tasarlanmıştır.

1️⃣ Tek Tıkla Kurulum
chmod +x setup.sh
./setup.sh


Bu işlem:

Gerekli kütüphaneleri kurar

captured_videos klasörünü oluşturur

2️⃣ Uygulamayı Başlatma
python app.py


Sunucu varsayılan olarak 5000 portunda çalışır.

3️⃣ Test ve Kayıt İnceleme

Test cihazı tarayıcı üzerinden uygulamaya bağlanır

Kamera izni kullanıcının açık onayıyla verilir

Gelen medya verileri test amacıyla sunucuda işlenebilir

Kayıtlı test çıktıları:

captured_videos/video_xxxx.webm

📂 Proje Dosyalarının Görevleri

setup.sh → Kurulum otomasyonu

index.html → Kullanıcıya açık şekilde bildirilen test arayüzü ve PiP tetikleyici

app.py → Sunucu, veri iletimi ve test kayıt yönetimi

requirements.txt → Gerekli Python bağımlılıkları






                                                                                                                                
