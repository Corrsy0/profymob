# Kurulum

ProfyMob kurulumu oldukça basittir. Yazılım tek bir EXE dosyası olarak gelir ve herhangi bir ek kurulum gerektirmez.

## 📥 İndirme

1. [repoce.com](https://repoce.com) adresinden **ProfyMob.exe** dosyasını indirin
2. İndirilen dosyayı istediğiniz bir klasöre kaydedin (örn: `C:\ProfyMob\`)

## ⚙️ Sistem Gereksinimleri Kontrolü

Yazılımı çalıştırmadan önce sisteminizin aşağıdaki gereksinimleri karşıladığından emin olun:

### Minimum Gereksinimler
- **İşletim Sistemi**: Windows 10 veya üzeri (64-bit)
- **RAM**: 4GB
- **Boş Disk Alanı**: 500MB
- **İnternet**: Stabil ADSL bağlantısı
- **.NET Framework**: Windows 10/11'de zaten yüklü

### Önerilen Gereksinimler
- **İşletim Sistemi**: Windows 11 (64-bit)
- **RAM**: 8GB veya üzeri
- **Boş Disk Alanı**: 1GB
- **İnternet**: Fiber bağlantı (hızlı işlem için)

## 🚀 İlk Çalıştırma

### Adım 1: Dosyayı Çalıştırma

1. `ProfyMob.exe` dosyasına çift tıklayın
2. Windows SmartScreen uyarısı çıkarsa:
   - **"Daha fazla bilgi"** bağlantısına tıklayın
   - **"Yine de çalıştır"** butonuna tıklayın
3. Yazılım başlatılacaktır

**Not**: Windows Defender veya antivirüs yazılımınız uyarı verebilir. ProfyMob tamamen güvenli bir yazılımdır, dosyayı güvenli listesine ekleyebilirsiniz.

### Adım 2: İlk Açılış

İlk açılışta yazılım otomatik olarak gerekli klasörleri oluşturacaktır:

```
ProfyMob.exe
├── config.json          # Ayarlarınız
├── reports.json         # Rapor verileri
├── proxies.txt          # Proxy listesi
├── logs/                # Log dosyaları
└── reports/             # Dışa aktarılan raporlar
```

## 🔑 Gerekli Servisler

ProfyMob'u kullanmak için aşağıdaki servislere ihtiyacınız vardır:

### 1. Captcha Çözüm Servisi (ZORUNLU)

Aşağıdaki servislerden **birinin** API anahtarını almanız gerekmektedir:

#### 2captcha.com
- **Web**: [2captcha.com](https://2captcha.com)
- **Kayıt**: Üye olun ve hesabınıza para yükleyin
- **API Key**: Dashboard > API Key bölümünden alın

#### Anti-Captcha.com
- **Web**: [anti-captcha.com](https://anti-captcha.com)
- **Kayıt**: Üye olun ve bakiye ekleyin
- **API Key**: Settings > API Key

#### CapSolver.com
- **Web**: [capsolver.com](https://capsolver.com)
- **Kayıt**: Kayıt olun ve bakiye yükleyin
- **API Key**: Dashboard'dan alın

#### CapMonster.cloud
- **Web**: [capmonster.cloud](https://capmonster.cloud)
- **Kayıt**: Hesap oluşturun
- **API Key**: Profile > API Key

### 2. Email Servisi (ZORUNLU)

Email doğrulaması gereken platformlar için **mutlaka** bir email servisi seçmelisiniz:

**xmailhub.net** (Önerilen)
- **Web**: [xmailhub.net](https://xmailhub.net)
- **Özellik**: Hızlı, güvenilir, 7/24 destek
- **API Key**: Dashboard'dan alın

**lution.ee**
- **Web**: [lution.ee](https://lution.ee)
- **Özellik**: Hızlı email teslimi
- **API Key**: Kayıt sonrası alın

**zeus-x.ru**
- **Web**: [zeus-x.ru](https://zeus-x.ru)
- **Özellik**: Rus platformlar için ideal
- **API Key**: Dashboard'dan alın

### 3. Proxy (OPSİYONEL AMA ÖNERİLİR)

Büyük miktarda işlem yapacaksanız proxy kullanımı önerilir:

- **HTTP/HTTPS Proxy**: Genel kullanım için
- **Formatlar**: 
  - `ip:port`
  - `ip:port:username:password`
  - `http://ip:port`

**Önerilen Proxy Servisleri**:
1. [we1.town](https://we1.town)
2. [dataimpulse.com](https://dataimpulse.com)
3. [proxycin.com](https://proxycin.com)

## ✅ Kurulum Tamamlandı

Kurulum tamamlandı! Şimdi [İlk Kullanım](first-use.md) kılavuzuna geçebilirsiniz.

## 🔧 Sorun Giderme

### Windows SmartScreen Uyarısı
**Sorun**: "Windows bu uygulamayı koruyarak bilgisayarınızı korudu" mesajı
**Çözüm**: 
1. "Daha fazla bilgi" bağlantısına tıklayın
2. "Yine de çalıştır" butonuna tıklayın

### Antivirüs Uyarısı
**Sorun**: Antivirüs yazılımı ProfyMob.exe'yi engelledi
**Çözüm**:
1. Antivirüs ayarlarını açın
2. ProfyMob.exe'yi güvenli listesine ekleyin
3. Dosyayı tekrar çalıştırın

### "VCRUNTIME140.dll eksik" Hatası
**Sorun**: VCRUNTIME140.dll bulunamadı hatası
**Çözüm**:
1. [Microsoft Visual C++ Redistributable](https://aka.ms/vs/17/release/vc_redist.x64.exe) indir ve yükle
2. Bilgisayarı yeniden başlat
3. ProfyMob'u tekrar çalıştır

### Yazılım Açılmıyor
**Sorun**: ProfyMob.exe'ye çift tıkladığımda hiçbir şey olmuyor
**Çözüm**:
1. `ProfyMob.exe` dosyasına sağ tıklayın
2. "Özellikler" > "Genel" sekmesine gidin
3. "Engeli kaldır" kutusunu işaretleyin
4. "Tamam" butonuna tıklayın
5. Dosyayı tekrar çalıştırın

### "Erişim Engellendi" Hatası
**Sorun**: Yazılım başlatılırken erişim engellendi hatası
**Çözüm**:
1. ProfyMob.exe'ye sağ tıklayın
2. "Yönetici olarak çalıştır" seçeneğini seçin

## 📞 Destek

Kurulum sırasında sorun yaşıyorsanız:
- **Web**: [repoce.com](https://repoce.com)
- **Dokümantasyon**: [Sık Sorulan Sorular](../reference/faq.md)

---

**Sonraki Adım**: [İlk Kullanım Kılavuzu](first-use.md)

