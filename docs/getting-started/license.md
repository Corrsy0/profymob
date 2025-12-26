# Lisans Aktivasyonu

ProfyMob lisanslı bir yazılımdır. Kullanmak için geçerli bir lisans anahtarına ihtiyacınız vardır.

## 🛒 Lisans Satın Alma

### Lisans Türleri

| Lisans Tipi | Süre | Fiyat | Özellikler |
|-------------|------|-------|-----------|
| **Aylık** | 30 gün | $XX | 1 bilgisayar, tüm platformlar |
| **3 Aylık** | 90 gün | $XX | 1 bilgisayar, tüm platformlar, %15 indirim |
| **Yıllık** | 365 gün | $XX | 1 bilgisayar, tüm platformlar, %30 indirim |
| **Ömür Boyu** | Sınırsız | $XX | 1 bilgisayar, tüm platformlar, tüm güncellemeler |

### Satın Alma Adımları

1. [repoce.com](https://repoce.com) adresini ziyaret edin
2. **"Lisans Satın Al"** butonuna tıklayın
3. İstediğiniz lisans tipini seçin
4. Ödeme bilgilerinizi girin
5. Ödeme tamamlandıktan sonra lisans anahtarınız email'inize gelecektir

**Kabul Edilen Ödeme Yöntemleri**:
- Kredi Kartı (Visa, MasterCard, American Express)
- PayPal
- Kripto Para (Bitcoin, Ethereum, USDT)
- Banka Havalesi (Türkiye için)

## 🔑 Lisans Aktivasyonu

### İlk Aktivasyon

1. `ProfyMob.exe` dosyasını çalıştırın
2. Lisans giriş ekranı açılacaktır
3. Email'inize gelen lisans anahtarını kopyalayın
4. Metin kutusuna yapıştırın
5. **"Giriş Yap"** butonuna tıklayın

![Lisans Girişi](../images/license-input.png)

**Lisans Format**: `XXXX-XXXX-XXXX-XXXX`

### Doğrulama Süreci

Lisans girişinden sonra yazılım:

1. ✅ İnternet bağlantısını kontrol eder
2. ✅ Lisans anahtarını backend sunucudan doğrular
3. ✅ Bilgisayarınızın HWID'sini (Hardware ID) oluşturur
4. ✅ Lisansı HWID ile eşleştirir
5. ✅ Lisans son kullanma tarihini kontrol eder
6. ✅ Ana sayfaya yönlendirir

**Süre**: 2-5 saniye

## 🔐 HWID (Hardware ID) Nedir?

### Tanım

HWID (Hardware ID), bilgisayarınızın benzersiz kimliğidir. ProfyMob lisansınızı belirli bir bilgisayara bağlar.

### Nasıl Oluşturulur?

HWID şu bilgilerden oluşturulur:
- CPU ID
- Motherboard Serial Number
- MAC Address
- Windows Ürün Anahtarı

### Neden Gerekli?

- **Güvenlik**: Lisansınızın başkaları tarafından kullanılmasını önler
- **Koruma**: Her lisans sadece 1 bilgisayarda çalışabilir
- **Yönetim**: Lisans durumunuzu merkezi olarak yönetebilirsiniz

## 📊 Lisans Durumu Kontrolü

### Lisans Bilgilerini Görüntüleme

Ana sayfa > **"Lisans Bilgileri"** bölümü:

```
📋 Lisans Bilgileri
━━━━━━━━━━━━━━━━━━━━
Email: user@example.com
Son Kullanma: 2025-12-31
Kalan Gün: 365 gün
Durum: ✅ Aktif
```

### Durum Göstergeleri

| Gösterge | Anlamı |
|----------|--------|
| ✅ **Aktif** | Lisansınız geçerli ve kullanılabilir |
| ⚠️ **Son 7 Gün** | Lisansınızın süresi 7 gün içinde dolacak |
| ❌ **Süresi Dolmuş** | Lisansınızı yenilemeniz gerekiyor |
| 🔒 **Bloke** | Lisansınız askıya alınmış (destek ile iletişime geçin) |

## 🔄 Lisans Yenileme

### Süre Dolmadan Yenileme

1. [repoce.com](https://repoce.com) hesabınıza giriş yapın
2. **"Lisanslarım"** bölümüne gidin
3. **"Yenile"** butonuna tıklayın
4. Ödemeyi tamamlayın
5. Lisans süresi otomatik uzayacaktır

**Not**: Aynı lisans anahtarını kullanmaya devam edebilirsiniz, yeni anahtar gerekmez.

### Süre Dolduktan Sonra

1. Yazılım "Lisans süresi dolmuş" hatası verecektir
2. repoce.com'dan yenileme yapın
3. Yazılımı yeniden başlatın
4. Otomatik olarak aktif olacaktır

## 💻 Bilgisayar Değiştirme

### Yeni Bilgisayara Taşıma

Eğer bilgisayarınızı değiştirdiyseniz:

1. [repoce.com](https://repoce.com) hesabınıza giriş yapın
2. **"Lisanslarım"** > **"HWID Sıfırla"** butonuna tıklayın
3. Eski bilgisayar bağlantısı kopar
4. Yeni bilgisayarda ProfyMob'u çalıştırın
5. Aynı lisans anahtarını girin
6. Yeni bilgisayar HWID'si ile eşleşecektir

**Sınırlama**: HWID sıfırlama ayda 1 kez yapılabilir.

### Format Sonrası

Windows format attıysanız:

1. HWID değişmiş olabilir
2. HWID sıfırlama işlemi yapın
3. Aynı lisans anahtarını tekrar girin

**İpucu**: Format atmadan önce lisans anahtarınızı yedekleyin.

## ❌ Lisans Hataları ve Çözümleri

### "Geçersiz lisans anahtarı"

**Sebep**: Yanlış format veya hatalı karakter
**Çözüm**:
1. Lisans anahtarını tekrar kopyalayın
2. Boşluk veya özel karakter olmadığından emin olun
3. Büyük/küçük harf önemli değil
4. Format: `XXXX-XXXX-XXXX-XXXX`

### "Lisans başka bilgisayarda kullanılıyor"

**Sebep**: Lisans farklı bir HWID'ye bağlı
**Çözüm**:
1. repoce.com'dan HWID sıfırlama yapın
2. 10 dakika bekleyin
3. Tekrar giriş yapın

### "Lisans süresi dolmuş"

**Sebep**: Lisans kullanım süresi sona ermiş
**Çözüm**:
1. repoce.com'dan lisans yenileme yapın
2. Ödemeyi tamamlayın
3. Yazılımı yeniden başlatın

### "İnternet bağlantısı hatası"

**Sebep**: Backend sunucusuna erişilemiyor
**Çözüm**:
1. İnternet bağlantınızı kontrol edin
2. Firewall/Antivirus ayarlarınızı kontrol edin
3. `backend.repoce.com` adresine erişebildiğinizden emin olun
4. VPN kullanıyorsanız kapatın

### "Lisans bloke edilmiş"

**Sebep**: Lisans kuralları ihlal edilmiş (paylaşım, kötüye kullanım vb.)
**Çözüm**:
1. repoce.com destek ile iletişime geçin
2. Durumu açıklayın
3. Destek ekibi inceleme yapacaktır

## 🛡️ Lisans Güvenliği

### Lisansınızı Koruma

1. ✅ Lisans anahtarınızı kimseyle paylaşmayın
2. ✅ Güvenli bir yerde saklayın (şifre yöneticisi)
3. ✅ Email'inizi düzenli kontrol edin
4. ✅ Şüpheli aktivite görürseniz hemen bildirin

### Yasak Eylemler

❌ Lisansı başkalarıyla paylaşmak
❌ Birden fazla bilgisayarda kullanmak
❌ Lisansı satmak veya kiralamak
❌ HWID sınırlamalarını bypass etmeye çalışmak
❌ Yazılımı tersine mühendislik yapmak

**Uyarı**: Bu eylemlerin tespiti durumunda lisansınız kalıcı olarak bloke edilecektir.

## 📧 Lisans Desteği

### Self-Servis

- **Portal**: [repoce.com](https://repoce.com)
- **İşlemler**: HWID sıfırlama, lisans yenileme, fatura görüntüleme

### Canlı Destek

Lisans ile ilgili sorunlarınız için:
- **Web**: repoce.com/destek
- **Email**: support@repoce.com
- **Yanıt Süresi**: 24 saat içinde

### Yaygın Destek Talepleri

1. HWID sıfırlama (self-servis ile yapılabilir)
2. Lisans yenileme (self-servis ile yapılabilir)
3. Fatura talebi
4. Lisans transferi (ücretli)
5. Toplu lisans satın alma (indirim için iletişime geçin)

## 💰 Fiyatlandırma ve İadeler

### İade Politikası

- **14 Gün**: Satın alma tarihinden itibaren 14 gün içinde iade yapabilirsiniz
- **Şartlar**: Yazılım kullanılmamış olmalı (ilk login sonrası iade geçersiz)
- **İşlem Süresi**: 5-7 iş günü

### İndirim Kodları

Özel günlerde ve kampanyalarda indirim kodları sunulmaktadır:
- Newsletter'a abone olun
- Sosyal medya hesaplarımızı takip edin
- repoce.com/kampanyalar sayfasını kontrol edin

## ❓ Sık Sorulan Sorular

### Lisansım birden fazla bilgisayarda çalışır mı?
Hayır, her lisans sadece 1 bilgisayarda çalışabilir. Birden fazla bilgisayarda kullanmak için ek lisans satın almanız gerekmektedir.

### Format attıktan sonra lisansım çalışır mı?
Evet, ancak HWID değişmiş olabilir. HWID sıfırlama yapmanız gerekebilir.

### Lisans sürem bittikten sonra oluşturduğum backlink'ler silinir mi?
Hayır, oluşturduğunuz backlink'ler platformlarda kalır. Sadece yeni backlink oluşturamazsınız.

### Ömür boyu lisans gerçekten ömür boyu mu?
Evet, bir kez ödeme yaparsınız ve yazılımı sonsuza kadar kullanabilirsiniz. Tüm güncellemeler dahildir.

### Lisansımı başka birine devredebilir miyim?
Lisans transferi ücretlidir. Destek ekibi ile iletişime geçin.

## 📚 İlgili Sayfalar

- [Kurulum](installation.md)
- [İlk Kullanım](first-use.md)
- [Sık Sorulan Sorular](../reference/faq.md)
- [Hata Kodları](../reference/error-codes.md)

---

**Önceki**: [İlk Kullanım](first-use.md) | **Sonraki**: [Arayüz Tanıtımı](../user-guide/interface.md)
