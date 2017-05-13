# MyBB-Oyuncu-Siyah
Tüm dosyaları **FTP**'de **MyBB**'nin bulunduğu klasöre yüklemeniz yeterli.
Ardından aşağıda ki eklentileri aktif ediniz ;

- Avatarep
- PHP and Template Conditionals

 
Herşey tamam, güncellemeleri buradan takip edebilirsiniz.
## Kendi sunucularımı nasıl eklerim ?
Anadizinde ki s1.php, s2.php, s3.php ve s4.php'yi açıp ip adresi kısmına kendi sunucumuzun ip'sini giriyoruz. (Sadece valve oyunları çalışıyor.)
### Tabi bunu kullanabilmek için tema içerisinde php kullanım iznine sahip olmanız gerekiyor. Peki bunu nasıl yapacaksınız ?
Zip dosyasının içerisinde inc/plugins klasöründe bu izne sahip olmanızı sağlıyacak eklenti mevcut, Eklenti yönetiminden -> PHP and Template Conditionals adlı eklentiyi aktif etmeniz yeterli.([Eklentinin orjinali için buraya tıklayınız.](http://community.mybb.com/thread-31860.html))

## Profilde kapak fotoğrafı olsun istiyorsanız ;
Admin paneline girip forum ayarları -> Özel profil yönetimi -> yeni profil alanı ekle diyoruz.

    Profil başlığı                : Kapak Fotoğrafı
    Kısa bilgi                     : Size kalmış
    Alan seçenekleri          : Text Kutusu
    Düzenli ifade               : Boş bırakın
    Maksimum uzunluk     : 500
    Minimum Mesaj Sayısı : 0
    Görüntülenme Sırası    : Size kalmış (Bende 0)
    Gerekli?                       : Kayıt sırasında ve Profil Bilgilerini Düzenleme kısmında bu alanı zorunlu olarak girdirmek istiyorsanız Evet deyin.
    Görüntüleme izinleri     : Tüm gruplar
    Düzenleme İzinleri       : Tüm gruplar

Diyoruz. Oluşturduğumuz Özel profilin üzerine gelip fid sayısını buluyoruz. (Üzerine gelince aşağıda edit&fid4 gibi bir yazı çıkar burda fid numaramız 4 bunu aklımızda tutuyoruz.)

**Temalar&Şablonlar -> Şablonlar -> Üye Profili Şablonlar -> member_profile** açıyoruz.
 **{$userfields['fid4']}** bunu aratın ve az önce bulduğumuz fid numarasını **4** yazan alana giriyoruz.


