# Hata Mesajları ve Çözümleri

Bu sayfa ProfyMob kullanırken karşılaşabileceğiniz hata mesajları ve çözümlerini içerir.

## 🔴 Kritik Hatalar

### "Lisans geçersiz" / "Invalid license key"

**Hata Kodu**: `LICENSE_INVALID`

**Sebep**:
- Yanlış lisans anahtarı
- Lisans format hatası
- Kopyala-yapıştır sırasında fazladan karakter

**Çözüm**:
1. Lisans anahtarınızı tekrar kopyalayın
2. Boşluk veya özel karakter olmadığından emin olun
3. Format: `XXXX-XXXX-XXXX-XXXX` (4 blok, her biri 4 karakter)
4. Büyük/küçük harf önemli değil

**Devam eden sorun**:
- Email'inizde lisans anahtarını kontrol edin
- [repoce.com](https://repoce.com) hesabınızdan lisansınızı görüntüleyin

---

### "Lisans süresi dolmuş" / "License expired"

**Hata Kodu**: `LICENSE_EXPIRED`

**Sebep**:
Lisans kullanım süresi sona ermiş

**Çözüm**:
1. [repoce.com](https://repoce.com) hesabınıza giriş yapın
2. "Lisanslarım" bölümüne gidin
3. "Yenile" butonuna tıklayın
4. Ödeme işlemini tamamlayın
5. Yazılımı yeniden başlatın

**Not**: Aynı lisans anahtarını kullanmaya devam edebilirsiniz

---

### "Lisans başka bilgisayarda kullanılıyor"

**Hata Kodu**: `LICENSE_ALREADY_USED`

**Sebep**:
Lisansınız farklı bir HWID (Hardware ID) ile eşleştirilmiş

**Çözüm**:
1. [repoce.com](https://repoce.com) hesabınıza giriş yapın
2. "Lisanslarım" > "HWID Sıfırla" tıklayın
3. 10 dakika bekleyin
4. ProfyMob'u tekrar çalıştırın
5. Lisans anahtarınızı girin

**Sınırlama**: HWID sıfırlama ayda 1 kez yapılabilir

---

### "Lisans bloke edilmiş"

**Hata Kodu**: `LICENSE_BLOCKED`

**Sebep**:
- Kullanım kurallarının ihlali
- Lisans paylaşımı
- Şüpheli aktivite

**Çözüm**:
1. repoce.com destek ile iletişime geçin
2. Durumu açıklayın
3. Destek ekibi inceleme yapacaktır

**Yasak Eylemler**:
- Lisansı birden fazla kişi kullanması
- HWID sınırlamalarını bypass etme
- Yazılımı tersine mühendislik

---

## 🌐 İnternet ve Bağlantı Hataları

### "İnternet bağlantısı hatası"

**Hata Kodu**: `NETWORK_ERROR`

**Sebep**:
- İnternet bağlantısı yok
- Backend sunucusuna erişilemiyor
- Firewall/Antivirus engelliyor

**Çözüm**:
1. İnternet bağlantınızı test edin (tarayıcıda google.com açın)
2. Firewall ayarlarını kontrol edin:
   - Windows Defender Firewall > "Bir uygulamaya izin ver"
   - ProfyMob.exe'yi ekleyin
3. Antivirüs yazılımını geçici olarak kapatın ve deneyin
4. VPN kullanıyorsanız kapatın

---

### "Proxy bağlantı hatası"

**Hata Kodu**: `PROXY_CONNECTION_ERROR`

**Sebep**:
- Proxy çalışmıyor
- Yanlış proxy formatı
- Authentication bilgileri hatalı

**Çözüm**:
1. Proxy'yi tarayıcıda test edin
2. Format kontrolü:
   ```
   Doğru: 123.456.789.012:8080
   Doğru: 123.456.789.012:8080:user:pass
   Doğru: http://123.456.789.012:8080
   
   Yanlış: 123.456.789.012 (port yok)
   Yanlış: http://123.456.789.012 (port yok)
   ```
3. Kullanıcı adı/şifre doğru mu kontrol edin
4. Farklı bir proxy deneyin

**Test**:
```
Tarayıcı > Ayarlar > Proxy ayarları
Proxy'nizi manuel ekleyin
google.com'u açmaya çalışın
Açılıyorsa proxy çalışıyor
```

---

### "Zaman aşımı" / "Timeout error"

**Hata Kodu**: `TIMEOUT_ERROR`

**Sebep**:
- İnternet çok yavaş
- Platform yanıt vermiyor
- Email doğrulama bekleniyor (60s)

**Çözüm**:
1. İnternet hızınızı test edin (speedtest.net)
2. Tekrar deneyin
3. Farklı platform seçin

**Normal Timeout Süreleri**:
- Platform istekleri: 10-20 saniye
- Email doğrulama: 60 saniye
- Captcha çözümü: 10 saniye

---

## 🔐 Captcha Hataları

### "Captcha çözülemedi"

**Hata Kodu**: `CAPTCHA_FAILED`

**Sebepler ve Çözümleri**:

#### 1. Bakiye Yetersiz
**Kontrol**:
- Ana sayfa > Captcha servisi > "Bakiye Kontrol" butonu

**Çözüm**:
- Captcha servisi hesabınıza bakiye yükleyin
- Minimum $2 bakiye önerilir

#### 2. Yanlış API Key
**Kontrol**:
- API key'i captcha servisi dashboard'undan tekrar kopyalayın

**Çözüm**:
- Ana sayfa > Captcha API Key kutusuna yapıştırın
- "Bakiye Kontrol" ile test edin

#### 3. Servis Çökmüş
**Kontrol**:
- Captcha servisi website'ını ziyaret edin
- Status page'i kontrol edin

**Çözüm**:
- Farklı bir captcha servisi seçin
- Birkaç dakika bekleyin ve tekrar deneyin

#### 4. Site Key Değişmiş
**Sebep**:
- Platform captcha site key'ini güncellemiş

**Çözüm**:
- Yazılım güncellemesini bekleyin
- repoce.com/destek adresine bildirin
- Farklı platform kullanın

---

### "Captcha zaman aşımı"

**Hata Kodu**: `CAPTCHA_TIMEOUT`

**Sebep**:
Captcha 120 saniye içinde çözülemedi

**Çözüm**:
1. Tekrar deneyin (bazen servis yavaş olabilir)
2. Farklı captcha servisi deneyin
3. İnternet hızınızı kontrol edin

**Captcha Çözüm Süreleri**:
- reCAPTCHA v2: 10-30 saniye
- reCAPTCHA v3: 5-15 saniye
- hCaptcha: 15-40 saniye

---

## 📧 Email Hataları

### "Email oluşturulamadı"

**Hata Kodu**: `EMAIL_CREATION_FAILED`

**Sebepler**:
 
- Yanlış API key
- Bakiye yetersiz

**Çözüm**:
1. API key'i kontrol edin
2. Email servisi dashboard'unuzu kontrol edin
3. Bakiye varsa servise destek talebi açın

---

### "Email doğrulama zaman aşımı"

**Hata Kodu**: `EMAIL_VERIFICATION_TIMEOUT`

**Sebep**:
60 saniye içinde doğrulama emaili gelmedi

**Çözümler**:

#### Kısa Vadeli
1. Tekrar deneyin (bazen gecikmeli gelir)
2. Farklı platform deneyin

#### Uzun Vadeli
Ücretli email servisi kullanın:
   - xmailhub.net (%99 güvenilir)
   - lution.ee
   - zeus-x.ru

---

### "Email inbox okunamadı"

**Hata Kodu**: `EMAIL_INBOX_ERROR`

**Sebep**:
Email servisi API'sine erişilemiyor

**Çözüm**:
1. İnternet bağlantınızı kontrol edin
2. Email servisi status page'ini kontrol edin
3. API key'i kontrol edin
4. Tekrar deneyin

---

## 🌍 Platform Hataları

### "Hesap oluşturulamadı"

**Hata Kodu**: `ACCOUNT_CREATION_FAILED`

**Sebepler ve Çözümleri**:

#### 1. Captcha Hatası
- Yukarıdaki captcha çözümlerini uygulayın

#### 2. Email Zaten Kullanılıyor
- Normal (rastgele email oluşturur, çakışma nadir)
- Tekrar deneyin

#### 3. IP Banlandı
**Sebep**: Çok fazla istek

**Çözüm**:
- Proxy kullanın
- Birkaç saat bekleyin
- Farklı platform deneyin

#### 4. Platform Değişiklik Yapmış
**Sebep**: Platform kayıt sürecini güncellemiş

**Çözüm**:
- Yazılım güncellemesini bekleyin
- repoce.com/destek adresine bildirin
- Farklı platform kullanın

---

### "Profil düzenlenemedi"

**Hata Kodu**: `PROFILE_EDIT_FAILED`

**Sebep**:
- Authentication problemi
- Platform oturum kapalı

**Çözüm**:
1. Tekrar deneyin
2. Farklı platform deneyin
3. Yazılım güncellemesini kontrol edin

**Not**: Hesap oluşturulmuştur, sadece profil düzenleme başarısız oldu. Hesap bilgilerini raporda bulabilir ve manuel düzenleyebilirsiniz.

---

### "Platform erişilemez"

**Hata Kodu**: `PLATFORM_UNREACHABLE`

**Sebep**:
- Platform çökmüş
- Bakımda
- Cloudflare koruması devrede

**Çözüm**:
1. Platform'un website'ını tarayıcıda açın
2. Çökmüş/bakımdaysa birkaç saat bekleyin
3. Farklı platform kullanın
4. Proxy kullanın (Cloudflare ise)

---

## 💾 Dosya ve Veri Hataları

### "config.json okunamadı"

**Hata Kodu**: `CONFIG_READ_ERROR`

**Sebep**:
- Dosya bozuk
- JSON format hatası
- Dosya başka program tarafından kilitli

**Çözüm**:
1. `config.json` dosyasını Notepad++ ile açın
2. JSON validator ile kontrol edin (jsonlint.com)
3. Eğer bozuksa dosyayı silin (yazılım yeni oluşturacak)
4. Ayarlarınızı tekrar girmeniz gerekecek

**Yedekleme**:
```
config.json.backup olarak yedekleyin
Sorun çıkarsa geri yükleyin
```

---

### "reports.json yazılamadı"

**Hata Kodu**: `REPORT_WRITE_ERROR`

**Sebep**:
- Dosya salt okunur
- Yetersiz disk alanı
- İzin problemi

**Çözüm**:
1. `reports.json` sağ tık > Özellikler
2. "Salt okunur" işaretini kaldırın
3. Disk alanını kontrol edin (en az 100MB boş)
4. Yönetici olarak çalıştırın

---

### "Rapor dışa aktarılamadı"

**Hata Kodu**: `EXPORT_FAILED`

**Sebepler**:

#### Excel Export
1. `reports/` klasörü yok
   - **Çözüm**: Manuel oluşturun
   
2. Dosya başka programda açık
   - **Çözüm**: Excel'i kapatın

3. openpyxl kütüphanesi hatası
   - **Çözüm**: Yazılımı yeniden indirin

#### PDF Export
1. ReportLab hatası
   - **Çözüm**: Yazılımı yeniden indirin

2. Font problemi
   - **Çözüm**: Windows fontlarını kontrol edin

---

## 🖥️ Sistem Hataları

### "VCRUNTIME140.dll eksik"

**Hata Kodu**: `VCRUNTIME_MISSING`

**Sebep**:
Visual C++ Redistributable yüklü değil

**Çözüm**:
1. [Microsoft Visual C++ Redistributable](https://aka.ms/vs/17/release/vc_redist.x64.exe) indir
2. Yükle
3. Bilgisayarı yeniden başlat
4. ProfyMob'u tekrar çalıştır

---

### "Uygulama yanıt vermiyor"

**Hata Kodu**: `APPLICATION_FREEZE`

**Sebep**:
- İşlem çok uzun sürüyor (normal)
- Deadlock (nadir)

**Çözüm**:
1. Bekleyin (email doğrulama 60s sürebilir)
2. Eğer 5 dakikadan fazla bekliyorsanız:
   - Task Manager > ProfyMob > "End Task"
   - Yazılımı tekrar başlatın

**Önleme**:
- Aynı anda çok fazla işlem başlatmayın
- İşlem tamamlanmadan yeni işlem başlatmayın

---

### "Bellek yetersiz"

**Hata Kodu**: `OUT_OF_MEMORY`

**Sebep**:
RAM yetersiz (nadir)

**Çözüm**:
1. Diğer programları kapatın
2. Tarayıcı sekmelerini azaltın
3. Bilgisayarı yeniden başlatın
4. RAM yükseltme düşünün (en az 8GB önerilir)

---

## ⚙️ Genel Sorun Giderme

### Genel Sorun Giderme Adımları

Herhangi bir hata için:

1. ✅ **Yazılımı Yeniden Başlat**
   - Çoğu geçici hata böyle çözülür

2. ✅ **İnternet Bağlantısını Kontrol Et**
   - google.com'u tarayıcıda açmayı dene

3. ✅ **Ayarları Kontrol Et**
   - Captcha API key doğru mu?
   - Email servisi seçili mi?
   - Proxy formatı doğru mu?

4. ✅ **Farklı Platform Dene**
   - Sorun platforma özgü olabilir

5. ✅ **Yazılımı Güncelle**
   - Yeni sürümü [repoce.com](https://repoce.com)'dan indir

6. ✅ **Destek İle İletişime Geç**
   - Yukarıdakilerin hiçbiri işe yaramadıysa

---

## 📊 Hata Kod Referansı

| Kod | Hata | Çözüm |
|-----|------|-------|
| `LICENSE_INVALID` | Geçersiz lisans | Lisans anahtarını kontrol edin |
| `LICENSE_EXPIRED` | Lisans dolmuş | Lisansı yenileyin |
| `LICENSE_ALREADY_USED` | Başka bilgisayarda | HWID sıfırlayın |
| `LICENSE_BLOCKED` | Lisans bloke | Destek ile iletişime geçin |
| `NETWORK_ERROR` | İnternet hatası | Bağlantıyı kontrol edin |
| `PROXY_CONNECTION_ERROR` | Proxy hatası | Proxy'yi test edin |
| `TIMEOUT_ERROR` | Zaman aşımı | Tekrar deneyin |
| `CAPTCHA_FAILED` | Captcha çözülemedi | Bakiye/API key kontrol |
| `CAPTCHA_TIMEOUT` | Captcha zaman aşımı | Farklı servis deneyin |
| `EMAIL_CREATION_FAILED` | Email oluşturulamadı | Ücretli servis kullanın |
| `EMAIL_VERIFICATION_TIMEOUT` | Email gelmedi | Ücretli servis kullanın |
| `EMAIL_INBOX_ERROR` | Inbox okunamadı | İnternet kontrol |
| `ACCOUNT_CREATION_FAILED` | Hesap oluşturulamadı | Proxy kullanın |
| `PROFILE_EDIT_FAILED` | Profil düzenlenemedi | Manuel düzenleyin |
| `PLATFORM_UNREACHABLE` | Platform erişilemez | Farklı platform |
| `CONFIG_READ_ERROR` | Config okunamadı | Dosyayı kontrol edin |
| `REPORT_WRITE_ERROR` | Rapor yazılamadı | İzinleri kontrol edin |
| `EXPORT_FAILED` | Export başarısız | Klasör var mı kontrol |
| `VCRUNTIME_MISSING` | DLL eksik | VC++ Redistributable yükleyin |
| `APPLICATION_FREEZE` | Yanıt vermiyor | Bekleyin veya yeniden başlatın |
| `OUT_OF_MEMORY` | Bellek yetersiz | RAM yükseltin |

---

## 📞 Hala Sorun mu Yaşıyorsunuz?

Eğer sorununuz bu sayfada yoksa veya çözüm işe yaramadıysa:

1. **Dokümantasyon**:
   - [Sık Sorulan Sorular](faq.md)
   - [Başlangıç Kılavuzu](../getting-started/installation.md)

2. **Destek**:
   - **Website**: [repoce.com/destek](https://repoce.com)
   - **Email**: support@repoce.com
   
3. **Destek Talebi Açarken Belirtin**:
   - Hata mesajı (tam metin)
   - Ne yaptığınızda hata oluştu
   - Ekran görüntüsü
   - İşletim sistemi ve versiyon
   - ProfyMob versiyonu

**Yanıt Süresi**: 24 saat içinde

---

