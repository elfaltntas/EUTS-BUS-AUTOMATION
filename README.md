# Elektronik Ücret Toplama Sistemi Otomasyonu

Bu proje, küçük ölçekli toplu taşıma sistemlerine uygun maliyetli ve kullanıcı dostu bir *Elektronik Ücret Toplama Sistemi (EÜTS)* geliştirmek amacıyla tasarlanmıştır. Sistem, *IoT* teknolojilerini kullanarak dijital ödeme ve araç takibi sağlar.

## Proje Özeti
*Elektronik Ücret Toplama Sistemi (EÜTS), **Raspberry Pi, **NFC kart okuyucu* ve *GPS modülü* entegre edilerek geliştirilmiştir. Sistem, yolcu kartlarını okuyarak ödeme alır, araç konumlarını izler ve bu bilgileri merkezi bir veri tabanına aktarır.

### Özellikler
- *IoT Tabanlı Çözüm:* NFC kart okuyucular ve GPS modülü ile veri toplama.
- *Raspberry Pi Altyapısı:* Ekonomik ve esnek donanım çözümü.
- *Python Yazılımı:* Algoritmalarla ödeme ve konum takibi.
- *Kullanıcı Dostu Arayüz:* Kart bakiye sorgulama ve yükleme.
- *Geleceğe Uyumlu:* QR kod ve mobil NFC entegrasyonuna uygun altyapı.

## Kullanılan Donanımlar
- *Raspberry Pi 4B (4GB)*
- *PN532 NFC Kart Okuyucu*
- *NEO-6M GPS Modülü*
- *7 inç Dokunmatik Ekran*

## Sistem Mimarisi
Sistem üç ana bileşenden oluşmaktadır:
1. *Otobüs Cihazı:* NFC okuyucular ve GPS modülü ile çalışır.
2. *Kullanıcı Arayüzü:* Kart bakiye sorgulama ve yükleme işlemleri.
3. *Kurumsal Yönetim Paneli:* Ödemeleri, konumları ve finansal işlemleri yönetir.

## Proje Kurulumu
### 1. Gerekli Yazılımların Kurulumu
- Raspberry Pi işletim sistemi: [Raspberry Pi OS](https://www.raspberrypi.com/software/)
- Python kütüphaneleri: pandas, flask, mysql-connector, pyserial
- Veri tabanı: *MySQL*

### 2. Donanım Bağlantıları
1. *NFC Modülü:* Raspberry Pi GPIO pinlerine bağlanır.
2. *GPS Modülü:* UART üzerinden bağlanır.
3. *Dokunmatik Ekran:* Raspberry Pi'nin DSI portu kullanılarak bağlanır.

### 3. Yazılım Kurulumu
1. Proje dosyalarını Raspberry Pi'ye klonlayın:
   bash
   git clone https://github.com/kullanici/EUTS.git
   cd EUTS
   
2. Gerekli Python kütüphanelerini yükleyin:
   bash
   pip install -r requirements.txt
   
3. Veri tabanı yapılandırmasını gerçekleştirin:
   bash
   mysql -u root -p < database/schema.sql
   
4. Uygulamayı başlatın:
   bash
   python main.py
   

## Kullanım
### 1. Otobüs Cihazı
- *Kart okutulduğunda:* Bakiye kontrolü yapılır, yeterli bakiye varsa ödeme alınır.
- *Konum takibi:* 2 saniyede bir GPS verisi merkezi sisteme gönderilir.

### 2. Kullanıcı Arayüzü
- *Bakiye Sorgulama:* Kullanıcılar T.C. kimlik numarası ile bakiye bilgilerini görebilir.
- *Bakiye Yükleme:* Kartlarına online bakiye yükleyebilirler.

### 3. Yönetim Paneli
- *Personel ve kart tanımlama.*
- *Araç konumlarının takibi.*
- *Gelir ve işlem raporları.*

## Test ve Değerlendirme
- *Fonksiyonel Testler:* Ödeme ve bakiye işlemlerinin doğruluğu test edilmiştir.
- *Güvenlik Testleri:* Veri şifreleme ile kullanıcı bilgileri korunmuştur.
- *Saha Testleri:* Gerçek otobüslerde sistem performansı değerlendirilmiştir.

## 📞 İletişim


- 📧 elfaltntas123@gmail.com  <br/>
Daha fazla bilgi için tıklayınız. <br/> [https://github.com/elfaltntas/EUTS-BUS-AUTOMATION/blob/main/BUS%20AUTOMATION.pdf]
