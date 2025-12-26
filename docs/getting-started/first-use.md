# İlk Kullanım

ProfyMob'u başarıyla kurduktan sonra, ilk kullanım adımlarını takip ederek yazılımı kullanmaya başlayabilirsiniz.

## 🔐 Lisans Aktivasyonu

### Adım 1: Yazılımı Başlatın

`ProfyMob.exe` dosyasını çift tıklayarak çalıştırın. İlk açılışta **Lisans Girişi** ekranı karşınıza gelecektir.

![Lisans Ekranı](../images/license-screen.png)

### Adım 2: Lisans Anahtarını Girin

1. Satın aldığınız lisans anahtarını metin kutusuna girin
2. Lisans formatı: `XXXX-XXXX-XXXX-XXXX`
3. **"Giriş Yap"** butonuna tıklayın

**Önemli**: 
- Lisans anahtarınız bulunduğunuz bilgisayara bağlıdır (HWID)
- Aynı lisansı farklı bilgisayarlarda kullanamazsınız
- Lisans bilgilerinizi güvenli bir yerde saklayın

### Adım 3: Lisans Doğrulama

Yazılım lisansınızı doğrulayacaktır:

✅ **Başarılı**: Ana sayfaya yönlendirileceksiniz
❌ **Başarısız**: Hata mesajını kontrol edin

**Olası Hatalar**:
- "Geçersiz lisans anahtarı" - Lisansınızı kontrol edin
- "Lisans süresi dolmuş" - Lisansınızı yenileyin
- "İnternet bağlantısı hatası" - İnternet bağlantınızı kontrol edin

## ⚙️ İlk Ayarlar

Lisans aktivasyonundan sonra ana sayfaya ulaşacaksınız. İlk olarak gerekli ayarları yapmanız gerekmektedir.

### Captcha Servisi Ayarlama

#### Adım 1: Ana Sayfa > Captcha Servisi Bölümü

1. **"Captcha Servisi Seç"** dropdown menüsünden servisinizi seçin:
   - 2captcha.com
   - anti-captcha.com
   - capsolver.com
   - capmonster.cloud

2. **"API Key"** kutusuna API anahtarınızı girin

3. **"Bakiye Kontrol"** butonuna tıklayarak bakiyenizi kontrol edin

![Captcha Ayarı](../images/captcha-settings.png)

#### Bakiye Göstergesi

✅ **Yeşil**: Bakiye yeterli (>$5)
⚠️ **Sarı**: Bakiye düşük ($1-$5)
❌ **Kırmızı**: Bakiye yetersiz (<$1)

**İpucu**: Bakiyeniz $5'in altına düştüğünde yeni bakiye yüklemeniz önerilir.

### Email Servisi Ayarlama (Opsiyonel)

#### Seçenek 1: Ücretsiz (mail.tm)

1. **"Email Servisi Seç"** dropdown'ından hiçbir şey seçmeyin
2. Yazılım otomatik olarak ücretsiz mail.tm kullanacaktır
3. API key gerekmez

**Avantajlar**:
- Ücretsiz
- Sınırsız kullanım

**Dezavantajlar**:
- Daha yavaş
- Bazen email gelmeyebilir
- Güvenilirlik düşük

#### Seçenek 2: Ücretli (Önerilir)

1. **"Email Servisi Seç"** dropdown'ından seçin:
   - xmailhub.net (Önerilir)
   - lution.ee
   - zeus-x.ru

2. **"API Key"** kutusuna API anahtarınızı girin

3. Ayarlar otomatik kaydedilir

**Avantajlar**:
- Çok hızlı (saniyeler içinde)
- %99 güvenilirlik
- 7/24 destek

![Email Ayarı](../images/email-settings.png)

### Proxy Ayarlama (Opsiyonel ama Önerilir)

#### Proxy Ekleme

1. Ana sayfa > **"Proxy Ayarları"** bölümü

2. **"Proxy Ekle"** butonuna tıklayın

3. Proxy bilgilerinizi girin:

**Desteklenen Formatlar**:
```
# Basit format
123.456.789.012:8080

# Kullanıcı adı ve şifre ile
123.456.789.012:8080:username:password

# HTTP protokolü ile
http://123.456.789.012:8080

# SOCKS5 protokolü ile
socks5://123.456.789.012:1080

# Authentication ile SOCKS5
socks5://username:password@123.456.789.012:1080
```

4. **"Kaydet"** butonuna tıklayın

#### Toplu Proxy Ekleme

Birden fazla proxy eklemek için:

1. `proxies.txt` dosyasını metin editörü ile açın (Notepad++)
2. Her satıra bir proxy yazın
3. Dosyayı kaydedin
4. Yazılımı yeniden başlatın

**proxies.txt örneği**:
```
123.456.789.012:8080
123.456.789.013:8080:user1:pass1
http://123.456.789.014:8080
socks5://123.456.789.015:1080
socks5://user2:pass2@123.456.789.016:1080
```

#### Proxy Test

Proxy'lerin çalıştığını test etmek için:
1. Herhangi bir platform seçin
2. Test işlemi başlatın
3. Konsol çıktısında proxy kullanımını göreceksiniz

**Not**: Yazılım proxy'leri otomatik olarak rotate eder, her istek farklı proxy kullanır.

## 📋 İlk Proje Oluşturma

Ayarlar tamamlandıktan sonra ilk projenizi oluşturabilirsiniz.

### Adım 1: Projeler Sayfasına Git

1. Sol menüden **"Projeler"** sekmesine tıklayın
2. **"Yeni Proje"** butonuna tıklayın

### Adım 2: Proje Bilgilerini Doldurun

![Proje Oluşturma](../images/create-project.png)

#### Gerekli Bilgiler:

**Temel Bilgiler**:
- **Proje Adı**: Projenizi tanımlayacak isim (örn: "Web Sitesi 1")
- **İsim Soyisim**: Profillerde kullanılacak isim (örn: "John Doe")
- **Cinsiyet**: Erkek / Kadın
- **Hakkında**: Profil açıklaması (100-500 karakter önerilir)

**Profil Fotoğrafı** (Opsiyonel):
- **"Resim Seç"** butonuna tıklayın
- Bilgisayarınızdan bir fotoğraf seçin
- Önerilen boyut: 400x400px
- Maksimum dosya boyutu: 2MB

**Backlink URL'leri**:
- **"Link Ekle"** butonuna tıklayın
- Web sitenizin URL'sini girin (örn: `https://example.com`)
- Birden fazla URL ekleyebilirsiniz
- En az 1, en fazla 10 URL önerilir

**Sosyal Medya Linkleri** (Opsiyonel):
- Twitter, Facebook, Instagram profil linkleriniz
- Bazı platformlar sosyal medya linklerini profilde gösterir

**Web 2.0 İçeriği**:
- **Blog Başlığı**: Blog yazısı başlığı
- **Blog İçeriği**: Makale içeriği (minimum 300 kelime önerilir)
- **Resimler**: Blog yazısına eklenecek görseller

**Yorum İçeriği**:
- **Yorum Metni**: WordPress bloglarına bırakılacak yorum
- Doğal ve alakalı yorumlar yazın
- Spam gibi görünmemesine dikkat edin

### Adım 3: Projeyi Kaydet

1. Tüm bilgileri doldurduktan sonra
2. **"Kaydet"** butonuna tıklayın
3. Proje listesinde görünecektir

## ✅ İlk Backlink Oluşturma

Artık ilk backlink'inizi oluşturmaya hazırsınız!

### Adım 1: Proje Seçimi

1. Sol menüden projenizi seçin
2. Proje detayları sağ tarafta görünecek

### Adım 2: İşlem Tipi Seçimi

ProfyMob 5 farklı backlink tipi sunar:

| Tip | Açıklama | Platform Sayısı |
|-----|----------|-----------------|
| **Profil** | Profil oluşturma ve backlink ekleme | 50+ |
| **Sosyal** | Sosyal işaretleme (bookmarking) | 10+ |
| **Web 2.0** | Blog yazısı yayınlama | 15+ |
| **Yorum** | WordPress blog yorumu | 5+ |
| **Forum** | Forum profil oluşturma | 10+ |

**İlk kullanım için "Profil" tipini öneriyoruz.**

### Adım 3: Platform Seçimi

1. **"İşlem Tipi"** olarak "Profil" seçin
2. **"Platform Seç"** dropdown menüsünden bir platform seçin:
   - Dev.to (Kolay, önerilir)
   - WordPress.org
   - Disqus.com
   - Pinterest.com
   - vb.

3. **"İşlem Sayısı"** girin (kaç tane profil oluşturulacak)
   - İlk denemede 1-2 önerilir
   - Maximum 100

### Adım 4: İşlemi Başlat

1. **"Başlat"** butonuna tıklayın
2. İşlem durumu ekranda görünecektir:
   - 🔄 Email oluşturuluyor...
   - 🔄 Hesap kaydediliyor...
   - 🔄 Email doğrulanıyor...
   - 🔄 Profil düzenleniyor...
   - ✅ Tamamlandı!

3. İşlem bittiğinde sonuç gösterilecektir

### Adım 5: Raporu İncele

1. **"Raporlar"** sekmesine gidin
2. Oluşturduğunuz profilleri göreceksiniz:
   - Profile URL
   - Email
   - Şifre
   - Kullanıcı adı

3. **"Excel"** veya **"PDF"** butonuna tıklayarak raporu indirebilirsiniz

## 🎉 Tebrikler!

İlk backlink'inizi başarıyla oluşturdunuz! Artık:

- Daha fazla platform deneyebilirsiniz
- İşlem sayısını artırabilirsiniz
- Farklı backlink tipleri (Sosyal, Web 2.0, Yorum) kullanabilirsiniz
- Toplu işlemler yapabilirsiniz

## 💡 İpuçları

### Başarı Oranını Artırma

1. **Kaliteli İçerik**: Profil açıklamanızı detaylı ve doğal yazın
2. **Gerçek Fotoğraf**: Profil fotoğrafı kullanın (stock photo değil)
3. **Çeşitlilik**: Farklı platformlar kullanın
4. **Proxy Kullanımı**: Büyük miktarda işlem yapıyorsanız proxy kullanın
5. **Yavaş İlerleyin**: Günde 10-20 backlink oluşturun (spam görünmemek için)

### Maliyet Optimizasyonu

1. **mail.tm Kullanın**: Çoğu platform için yeterlidir
2. **CapMonster Seçin**: En ucuz captcha servisi
3. **Proxy Paylaşımı**: Aynı proxy'leri farklı projelerde kullanın

### Güvenlik

1. **Farklı İsimler**: Her proje için farklı isim kullanın
2. **Değişken İçerik**: Her projede farklı açıklamalar yazın
3. **Doğal Backlink**: Alakalı ve değerli içerik oluşturun

## ❓ Sık Sorulan Sorular

### "Captcha çözülemedi" hatası alıyorum
**Çözüm**: 
- Captcha servisi bakiyenizi kontrol edin
- API anahtarınızın doğru olduğundan emin olun
- Farklı bir captcha servisi deneyin

### Email doğrulama zaman aşımı
**Çözüm**:
- Ücretli email servisi kullanın (xmailhub.net)
- İnternet hızınızı kontrol edin
- Tekrar deneyin

### "Proxy bağlantı hatası"
**Çözüm**:
- Proxy'nizin çalıştığını test edin
- Farklı bir proxy deneyin
- Proxy formatını kontrol edin

### İşlem çok yavaş ilerliyor
**Sebep**: 
- Email doğrulama bekleniyor (60 saniye timeout)
- Captcha çözülüyor (5-30 saniye)
- Platform yavaş yanıt veriyor

**Çözüm**:
- Normal, sabırlı olun
- Ücretli email servisi kullanın (daha hızlı)

## 📚 Sonraki Adımlar

- [Arayüz Tanıtımı](../user-guide/interface.md) - Tüm özellikleri öğrenin
- [Proje Yönetimi](../user-guide/projects.md) - İleri seviye proje ayarları
- [Profil Backlink](../user-guide/profile-backlinks.md) - Profil oluşturma detayları
- [Rapor Oluşturma](../user-guide/reports.md) - Rapor yönetimi

## 📞 Yardım

Herhangi bir sorunuz varsa:
- [Sık Sorulan Sorular](../reference/faq.md)
- [Hata Çözümleri](../reference/error-codes.md)
- [Web](https://repoce.com)

---

**Önceki**: [Kurulum](installation.md) | **Sonraki**: [Lisans Aktivasyonu](license.md)
