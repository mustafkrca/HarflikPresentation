#  <img src="https://github.com/mustafkrca/HarflikPresentation/blob/main/logo.png" alt="Harflik Logo" width="50" align="top"> Harflik

**Harflik**, oyuncuların her yaşta eğlenerek kelime bulmacaları çözebileceği, bağımlılık yapıcı bir oyun. 3 Ağustos 2024'te Google Play'de yayınlanacak olan bu oyun, yakın zamanda iOS platformunda da yerini alacak.

## Genel Bakış
Harflik, farklı kelimeler deneyerek harflerin konumuna göre yanan renge bakarak bulmaca tarzında doğru kelimeye ulaşma oyunudur.

## Ekran Görüntüleri
<div style="display: flex; flex-wrap: wrap; justify-content: space-between;">
    <img src="https://github.com/mustafkrca/HarflikPresentation/blob/main/img1.png" alt="Harflik Ana Menüsü" style="width: 23%; height: auto; margin: 1%;">
    <img src="https://github.com/mustafkrca/HarflikPresentation/blob/main/img2.png" alt="Oyun Ekranı" style="width: 23%; height: auto; margin: 1%;">
    <img src="https://github.com/mustafkrca/HarflikPresentation/blob/main/img3.png" alt="Günlük Meydan Okuma" style="width: 23%; height: auto; margin: 1%;">
    <img src="https://github.com/mustafkrca/HarflikPresentation/blob/main/img4.png" alt="Liderlik Tablosu" style="width: 23%; height: auto; margin: 1%;">
</div>

## Özellikler
- **Zaman Modu:** Son 8 saniye aktif olan geri sayım sesi ve kazanınca,kaybedince gelen ses efekti ekledim.
- **Kelime Optimizasyonu:** Çözülen Kelime bir daha aynı kullanıcıya sunulmuyor.
- **Api Optimizasyonu:** Api den her seferinde 10 kelime çağrılarak 10 kelime bittiğinde tekrar istek atılması ile sürekli istek atmanın önüne geçtim.
- **Reklamlar:** Uygulamaya Admob üzerinden reklam entegresi yaptım.
- **İpuçları:** İpuçlar arasında harf yardımı ve kelimenin anlamını gösteren butonlar ekledim.
- **Bildirimler:** Firebase Console entegresi ile anlık bildirim eklentisi yaptım.
- **Animasyonlar:** Lottie üzerinden ve gifler ile entegre edilmiş animasyonlar


## Geliştirme Süreci - Teknoloji Yığını

### Kelimelerin Üretilmesi
TDK'dan alınan yaklaşık 160.000 Türkçe kelime tek bir JSON dosyasına indirildi ve Zemberek NLP kütüphanesi kullanılarak işlendi. Kelimeler sıfat, fiil, isim olarak sınıflandırıldı ve isimlerden yaklaşık 8.000 adet kök elde edildi. Bu kelimeler 4, 5 ve 6 harfli olarak ayrıldı ve Python kullanılarak ayrı JSON dosyalarında saklandı. Ardından, Node.js kullanılarak TDK kütüphanesi ile bu kelimelerin anlamları bulundu ve tekrar JSON olarak oluşturuldu. Bu JSON dosyaları veritabanına aktarıldı.

### Frontend
- **React Native:** Sorunsuz ve duyarlı bir mobil uygulama deneyimi.
- **Firebase:** Bildirimler ve bulut işlevsellikleri için.
- **Lottie:** Animasyonları canlandırmak için.
- **AdMob:** Reklam entegrasyonu için.

### Backend
- **Node.js:** Kendi VDS sunucumda çalışmaktadır.

### Veritabanı
- **MongoDB:** Oyun verilerini (Kelime, Kelimenin Anlamı) depolamak için VDS sunucumda kuruludur.

### Kelimeler
- **Zemberek NLP:** Türkçe Doğal Dil işleme java kütüphanesi.

## İletişim
Herhangi bir soru veya geri bildirim için lütfen ulaşın:
- Uygulama : https://shorturl.at/siSrD
- Email: [mustafkrca@gmail.com](mailto:mustafkrca@gmail.com)
- LinkedIn: [LinkedIn](https://www.linkedin.com/in/mustafa-karaca-222804192/)

Kodlar hesabımda private olarak tutulmaktadır.
