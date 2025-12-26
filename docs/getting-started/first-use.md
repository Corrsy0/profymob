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

### Email Servisi Ayarlama (Zorunlu)

1. **"Email Servisi Seç"** dropdown'ından bir servis seçin:
   - xmailhub.net (Önerilir)
   - lution.ee
   - zeus-x.ru

2. **"API Key"** kutusuna API anahtarınızı girin

3. **"Bakiye Kontrol"** butonuna tıklayarak bakiyenizi kontrol edin

4. Ayarlar otomatik kaydedilir

**Özellikler**:
- Çok hızlı email teslimi (saniyeler içinde)
- Yüksek güvenilirlik
- Tüm platformlarda çalışır

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

**Not**: Yazılım proxy'leri otomatik olarak rotate eder, her istek farklı proxy kullanır.

## 📋 İlk Proje Oluşturma

Ayarlar tamamlandıktan sonra ilk projenizi oluşturabilirsiniz.

### Adım 1: Projeler Sayfasına Git

1. Sol menüden **"Projeler"** sekmesine tıklayın
2. **"Yeni Proje"** butonuna tıklayın

### Adım 2: Proje Bilgilerini Doldurun

![Proje Oluşturma](../images/create-project.png)

#### Gerekli Bilgiler:

**Proje Adı**:
- Projenizi tanımlayacak bir isim girin (örn: "Web Sitesi 1", "Müşteri X")
- Bu isim sadece siz görebilirsiniz, organizasyon için kullanılır

**Proje Ayarlarını Kaydetme**:
- Profil backlink sayfasında işlem bilgilerinizi (kullanıcı adı, açıklama, linkler vb.) girdikten sonra
- **"Ayarları Kaydet"** butonuna tıklayarak bu bilgileri projeye kaydedebilirsiniz
- Kaydedilen ayarlar, daha sonra aynı proje için tekrar kullanılabilir
- Her backlink tipi (Profil, Sosyal, Web 2.0, Yorum) için ayrı ayarlar kaydedebilirsiniz

### Adım 3: Projeyi Kaydet

1. Tüm bilgileri doldurduktan sonra
2. **"Kaydet"** butonuna tıklayın
3. Proje listesinde görünecektir

## ✅ İlk Backlink Oluşturma

Artık ilk backlink'inizi oluşturmaya hazırsınız!

### Adım 1: Proje Seçimi

1. Sol menüden projenizi seçin
2. Proje detayları sağ tarafta görünecek

### Adım 2: Backlink Sayfalarına Git

ProfyMob sol menüde 4 farklı backlink sayfası sunar:

| Sayfa | Açıklama | Platform Sayısı |
|-------|----------|-----------------|  
| **Profil Backlink** | Profil oluşturma ve backlink ekleme | 45+ |
| **Sosyal Backlink** | Sosyal işaretleme (bookmarking) | 10+ |
| **Web 2.0 Backlink** | Blog yazısı yayınlama | 15+ |
| **Yorum Backlink** | WordPress blog yorumu | 5+ |

**Not**: Forum backlink özelliği şu anda bakımda.

**İlk kullanım için "Profil Backlink" sayfasını öneriyoruz.**

### Adım 3: Platform Seçimi ve İşlem Başlatma

1. Sol menüden **"Profil Backlink"** sayfasına gidin
2. **"Platform Seç"** dropdown menüsünden bir platform seçin:
   - Dev.to (Kolay, önerilir)
   - WordPress.org
   - Disqus.com
   - Pinterest.com
   - vb.

3. Gerekli bilgileri doldurun (kullanıcı adı, açıklama, link vb.)
4. **"İşlem Sayısı"** girin (kaç tane profil oluşturulacak)
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
2. **Çeşitlilik**: Farklı platformlar kullanın
3. **Proxy Kullanımı**: Büyük miktarda işlem yapıyorsanız proxy kullanın
4. **Yavaş İlerleyin**: Günde 10-20 backlink oluşturun (spam görünmemek için)
5. **Servis Bakiyesi**: Captcha ve email servis bakiyenizi düzenli kontrol edin

### Güvenlik

1. **Farklı İsimler**: Her proje için farklı isim kullanın
2. **Değişken İçerik**: Her projede farklı açıklamalar yazın
3. **Doğal Backlink**: Alakalı ve değerli içerik oluşturun
4. **Proxy Kullanımı**: Büyük işlemler için mutlaka proxy kullanın

## ❓ Sık Sorulan Sorular

### "Captcha çözülemedi" hatası alıyorum
**Çözüm**: 
- Captcha servisi bakiyenizi kontrol edin
- API anahtarınızın doğru olduğundan emin olun
- Farklı bir captcha servisi deneyin

### Email doğrulama zaman aşımı
**Çözüm**:
- Email servisi bakiyenizi kontrol edin
- İnternet hızınızı kontrol edin
- Tekrar deneyin
- Farklı bir email servisi deneyin

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
- Hızlı email servisleri (xmailhub.net) daha hızlı sonuç verir

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
