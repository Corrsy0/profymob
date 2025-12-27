# Raporlar

ProfyMob, oluşturduğunuz tüm backlink'lerin detaylı raporlarını tutar. Raporları görüntüleyebilir, filtreleyebilir ve Excel/PDF formatında dışa aktarabilirsiniz.

## 📊 Rapor Sistemi

### Rapor Nedir?

Her başarılı backlink oluşturma işlemi için otomatik olarak bir rapor kaydı oluşturulur.

**Rapor İçeriği**:
- Platform adı
- Profile/Hesap URL'si
- Email adresi
- Şifre
- Kullanıcı adı
- Oluşturulma tarihi ve saati
- Proje adı
- Durum (Başarılı/Başarısız)
- İşlem süresi
- Kullanılan proxy (varsa)

### Raporlar Nasıl Saklanır?

**Yerel Depolama**:
- Tüm raporlar `reports.json` dosyasında saklanır
- Dosya yazılım klasöründe bulunur
- Otomatik olarak güncellenir
- Sadece bilgisayarınızda saklanır

**Güvenlik**:
- Şifreler düz metin olarak saklanır
- Dosyayı güvenli tutun
- Düzenli yedekleme yapın
- Paylaşmayın

## 📋 Raporlar Sayfası

### Ana Görünüm

Sol menüden **"Raporlar"** sekmesine tıklayarak raporlar sayfasına ulaşabilirsiniz.

**Tablo Sütunları**:
| Sütun | Açıklama |
|-------|----------|
| Durum | ✅ Başarılı / ❌ Başarısız |
| Platform | Platformun adı |
| Profil URL | Oluşturulan profil linki |
| Email | Kullanılan email adresi |
| Şifre | Hesap şifresi |
| Kullanıcı Adı | Hesap kullanıcı adı |
| Proje | Hangi projede oluşturuldu |
| Tarih | Oluşturulma tarihi |
| Süre | İşlem süresi (saniye) |

### Rapor Detayları

Bir rapora tıklayarak detaylı bilgileri görüntüleyebilirsiniz:

**Detay Penceresi**:
```
📋 Rapor Detayları
━━━━━━━━━━━━━━━━━━━━

Platform: Dev.to
Durum: ✅ Başarılı
Profil URL: https://dev.to/johndoe2025
Email: temp123@example.com
Şifre: SecurePass123!
Kullanıcı Adı: johndoe2025

Proje: Müşteri1-Profil-Backlinks
Oluşturulma: 27.12.2025 14:30:15
İşlem Süresi: 95 saniye

Captcha Servisi: 2captcha.com
Email Servisi: xmailhub.net
Proxy: http://proxy.example.com:8080

İşlem Adımları:
1. Email oluşturuldu (8 saniye)
2. Kayıt formu dolduruldu (12 saniye)
3. Captcha çözüldü (25 saniye)
4. Email doğrulandı (35 saniye)
5. Profil düzenlendi (15 saniye)

Notlar: -
```

## 🔍 Filtreleme ve Arama

### Hızlı Arama

**Arama Çubuğu**:
- Platform adıyla ara
- Email adresine göre ara
- Kullanıcı adına göre ara
- Proje adına göre ara
- URL'ye göre ara

**Örnek Aramalar**:
```
"dev.to" → Dev.to platformundaki tüm raporlar
"@example.com" → Belirli domain emaili içeren raporlar
"Müşteri1" → Belirli projede oluşturulan raporlar
"johndoe" → Kullanıcı adı içeren raporlar
```

### Gelişmiş Filtreler

#### Tarih Filtreleme

**Ön Tanımlı Aralıklar**:
- Bugün
- Dün
- Son 7 gün
- Son 30 gün
- Bu ay
- Geçen ay
- Tüm zamanlar

**Özel Tarih Aralığı**:
1. "Özel Aralık" seçin
2. Başlangıç tarihi seçin
3. Bitiş tarihi seçin
4. "Uygula" butonuna tıklayın

#### Platform Filtreleme

**Tek Platform**:
- Dropdown menüden platform seçin
- Sadece o platformun raporları gösterilir

**Çoklu Platform**:
- Birden fazla platform seçin (Ctrl+tıklama)
- Seçili platformların raporları gösterilir

#### Proje Filtreleme

**Tek Proje**:
- Dropdown menüden proje seçin
- Sadece o projenin raporları gösterilir

**Çoklu Proje**:
- Birden fazla proje seçin
- Seçili projelerin raporları gösterilir

#### Durum Filtreleme

**Filtre Seçenekleri**:
- ✅ Sadece Başarılı
- ❌ Sadece Başarısız
- 🔄 Tümü

### Sıralama

**Sıralama Seçenekleri**:
- Tarihe göre (Yeni → Eski)
- Tarihe göre (Eski → Yeni)
- Platforma göre (A-Z)
- Platforma göre (Z-A)
- Projeye göre (A-Z)
- Duruma göre (Başarılı önce)

## 📤 Dışa Aktarma (Export)

### Excel Export

**Adımlar**:
1. Export edilecek raporları filtreleyin (opsiyonel)
2. **"Excel Export"** butonuna tıklayın
3. Kaydetmek istediğiniz yeri seçin
4. Dosya adı girin (varsayılan: `profymob_rapor_YYYYMMDD_HHMMSS.xlsx`)
5. **"Kaydet"** butonuna tıklayın

**Excel İçeriği**:
- Tüm rapor alanları dahil
- Her satır bir backlink
- Başlık satırı dahil
- Filtreler uygulanmış

**Excel Sütunları**:
| Sütun | İçerik |
|-------|--------|
| A | Durum |
| B | Platform |
| C | Profil URL |
| D | Email |
| E | Şifre |
| F | Kullanıcı Adı |
| G | Proje |
| H | Oluşturulma Tarihi |
| I | İşlem Süresi |

**Kullanım Alanları**:
- Müşteri raporlama
- Backlink listeleme
- Veri analizi
- Yedekleme

### PDF Export

**Adımlar**:
1. Export edilecek raporları filtreleyin (opsiyonel)
2. **"PDF Export"** butonuna tıklayın
3. PDF ayarlarını yapın:
   - Logo ekle (opsiyonel)
   - Başlık metni
   - Alt bilgi
4. **"Oluştur"** butonuna tıklayın
5. Kaydetmek istediğiniz yeri seçin

**PDF İçeriği**:
- Profesyonel tasarım
- Logo ve başlık
- Tablo formatında raporlar
- Sayfa numaraları
- Oluşturulma tarihi
- Toplam istatistikler

**Kullanım Alanları**:
- Müşteri sunumları
- Profesyonel raporlar
- Yazdırma
- Arşivleme

### CSV Export

**Adımlar**:
1. Export edilecek raporları filtreleyin (opsiyonel)
2. **"CSV Export"** butonuna tıklayın
3. Ayırıcı seçin (virgül, noktalı virgül, tab)
4. Kaydetmek istediğiniz yeri seçin
5. **"Kaydet"** butonuna tıklayın

**CSV İçeriği**:
- Basit metin formatı
- Excel'de açılabilir
- Veritabanına import edilebilir

**Kullanım Alanları**:
- Veri taşıma
- Diğer yazılımlara import
- Veritabanı entegrasyonu

## 🗑️ Rapor Yönetimi

### Tek Rapor Silme

**Adımlar**:
1. Silinecek rapora tıklayın
2. **"Sil"** butonuna tıklayın
3. Onay mesajı: "Bu rapor silinecek, emin misiniz?"
4. **"Evet, Sil"** butonuna tıklayın

**Uyarı**: 
- Silinen rapor geri alınamaz
- Excel/PDF export'u yoksa veri kaybolur
- Dikkatli olun

### Toplu Silme

**Seçerek Silme**:
1. Silinecek raporları seçin (Ctrl+tıklama veya Shift+tıklama)
2. **"Seçilenleri Sil"** butonuna tıklayın
3. Onay mesajı: "X adet rapor silinecek, emin misiniz?"
4. **"Evet, Sil"** butonuna tıklayın

**Filtre ile Silme**:
1. Filtre uygulayın (örn: 30 günden eski raporlar)
2. **"Filtrelileri Sil"** butonuna tıklayın
3. Onay mesajı görünür
4. **"Evet, Sil"** butonuna tıklayın

**Tümünü Silme**:
1. **"Tüm Raporları Sil"** butonuna tıklayın
2. Onay mesajı: "TÜM RAPORLAR SİLİNECEK! Emin misiniz?"
3. Güvenlik sorusu: "Silmek için 'SIFIRLA' yazın"
4. "SIFIRLA" yazıp **"Onayla"** butonuna tıklayın

**Uyarı**: Bu işlem geri alınamaz!

### Rapor Düzenleme

**Düzenlenebilir Alanlar**:
- Notlar ekleyebilirsiniz
- Proje adını değiştirebilirsiniz
- Durum etiketleri ekleyebilirsiniz

**Düzenlenemeyen Alanlar**:
- Platform
- URL
- Email
- Şifre
- Tarih
- İşlem süresi

**Düzenleme Adımları**:
1. Rapora tıklayın
2. **"Düzenle"** butonuna tıklayın
3. Değiştirmek istediğiniz alanları düzenleyin
4. **"Kaydet"** butonuna tıklayın

## 📈 Rapor İstatistikleri

### Genel İstatistikler

Raporlar sayfasının üst kısmında genel istatistikler görüntülenir:

**Göstergeler**:
```
📊 Genel İstatistikler
━━━━━━━━━━━━━━━━━━━━

Toplam Backlink: 523
✅ Başarılı: 487 (93%)
❌ Başarısız: 36 (7%)

Bu Ay: 127 backlink
Bu Hafta: 43 backlink
Bugün: 12 backlink

En Çok Kullanılan Platform: Dev.to (89 backlink)
En Başarılı Platform: WordPress.org (98% başarı)
Ortalama İşlem Süresi: 102 saniye
```

### Platform Bazında İstatistikler

**Görüntüleme**:
1. **"Platform İstatistikleri"** butonuna tıklayın
2. Platform listesi görünür

**İçerik**:
| Platform | Toplam | Başarılı | Başarı Oranı | Ort. Süre |
|----------|--------|----------|--------------|-----------|
| Dev.to | 89 | 86 | 96.6% | 95 sn |
| WordPress.org | 67 | 66 | 98.5% | 110 sn |
| Pinterest.com | 54 | 48 | 88.9% | 85 sn |
| Disqus.com | 43 | 42 | 97.7% | 78 sn |

**Grafikler**:
- Pasta grafiği: Platform dağılımı
- Çubuk grafiği: Başarı oranları
- Çizgi grafiği: Zaman içinde trend

### Proje Bazında İstatistikler

**Görüntüleme**:
1. **"Proje İstatistikleri"** butonuna tıklayın
2. Proje listesi görünür

**İçerik**:
| Proje | Toplam | Platform Sayısı | Başarı Oranı | İlk İşlem | Son İşlem |
|-------|--------|-----------------|--------------|-----------|-----------|
| Müşteri1 | 156 | 12 | 94% | 01.11.2024 | 27.12.2025 |
| Web1 | 89 | 8 | 91% | 15.11.2024 | 25.12.2025 |
| Test | 23 | 5 | 78% | 20.12.2024 | 27.12.2025 |

### Zaman Bazında Analiz

**Görsel Gösterim**:
- Günlük backlink sayısı (son 30 gün)
- Haftalık trend
- Aylık karşılaştırma
- Başarı oranı trendi

**Örnek Grafik Verisi**:
```
Aralık 2025 - Günlük Backlink

27 Ara: ████████████ 12
26 Ara: ████████████████ 16
25 Ara: ████████ 8
24 Ara: ██████████████ 14
23 Ara: - 0 (Pazar)
...
```

## 💾 Yedekleme ve Geri Yükleme

### Manuel Yedekleme

**reports.json Dosyası**:
1. ProfyMob klasörünü açın
2. `reports.json` dosyasını bulun
3. Dosyayı kopyalayın
4. Güvenli bir yere kaydedin (cloud, USB vb.)

**Önerilen Yedekleme Sıklığı**:
- Günlük: Çok aktif kullanıyorsanız
- Haftalık: Normal kullanım
- Aylık: Az kullanım

**Yedekleme İsimlendirmesi**:
```
reports_20251227.json
reports_backup_27_12_2025.json
profymob_reports_2025_12_27.json
```

### Otomatik Yedekleme

**Ayarlama**:
1. Ayarlar > Yedekleme sekmesine gidin
2. **"Otomatik Yedekleme"** seçeneğini aktif edin
3. Yedekleme sıklığını seçin (Günlük/Haftalık/Aylık)
4. Yedekleme klasörünü seçin
5. **"Kaydet"**

**Otomatik Yedek Dosyaları**:
```
backups/
├── reports_2025_12_27.json
├── reports_2025_12_20.json
├── reports_2025_12_13.json
└── reports_2025_12_06.json
```

### Geri Yükleme

**Manuel Geri Yükleme**:
1. ProfyMob'u kapatın
2. Yedek `reports.json` dosyasını kopyalayın
3. Mevcut `reports.json` dosyasının yerine yapıştırın
4. ProfyMob'u başlatın

**Yazılım İçinden Geri Yükleme**:
1. Ayarlar > Yedekleme > **"Geri Yükle"** butonuna tıklayın
2. Yedek dosyayı seçin
3. Geri yükleme seçeneği seçin:
   - **"Üzerine Yaz"**: Mevcut raporlar silinir, yedek yüklenir
   - **"Birleştir"**: Yedek raporlar mevcut raporlara eklenir
4. **"Geri Yükle"** butonuna tıklayın

**Uyarı**: "Üzerine Yaz" seçeneği mevcut raporları siler!

## 🔒 Güvenlik ve Gizlilik

### Şifre Güvenliği

**Raporlarda Şifreler**:
- ❌ Şifrelenmiş DEĞİL
- ✅ Düz metin olarak saklanır
- ⚠️ Güvenli tutun

**Öneriler**:
1. `reports.json` dosyasını kimseyle paylaşmayın
2. Cloud yedekleme yapıyorsanız şifreli cloud kullanın
3. Bilgisayarınızı şifre ile koruyun
4. Güvenli yerden çalışın

### Veri Gizliliği

**Yerel Depolama**:
- Tüm raporlar sadece bilgisayarınızda
- Sunucuya gönderilmez
- İnternet gerektirmez (görüntüleme için)

**Export Güvenliği**:
- Excel/PDF dosyaları şifre korumalı yapılabilir
- Hassas bilgiler içerebilir
- Dikkatli paylaşın

## 💡 İpuçları ve Best Practices

### Organizasyon

1. **Düzenli Export**: Haftada bir Excel raporu alın
2. **Eski Raporları Temizleyin**: 6 ay önceki raporları silin
3. **Proje Bazlı Takip**: Her proje için ayrı rapor tutun
4. **Notlar Ekleyin**: Önemli backlinklere not ekleyin

### Analiz

1. **Başarı Oranını Takip Edin**: Platform başına başarı oranı
2. **En İyi Platformları Belirleyin**: Yüksek başarı oranına odaklanın
3. **Trend Analizi**: Zaman içinde backlink artışı
4. **Başarısızlık Sebeplerini Inceleyin**: Hangi platformlarda sorun var?

### Yedekleme

1. **Otomatik Yedekleme Kurun**: Veri kaybını önler
2. **Cloud Yedekleme**: Dropbox, Google Drive gibi
3. **Versiyonlama**: Eski yedekleri sakla
4. **Test Edin**: Geri yüklemenin çalıştığını test edin

### Performans

1. **Eski Raporları Arşivleyin**: Yazılım hızını artırır
2. **Filtreleri Kullanın**: Büyük listelerde arama yapın
3. **Excel Export**: Büyük analizler için Excel kullanın

## ❓ Sık Sorulan Sorular

### Kaç rapor saklayabilirim?
Sınır yok, ancak 10,000+ raporda performans düşebilir. Eski raporları arşivleyin.

### Raporları silebilir miyim?
Evet, tek tek veya toplu olarak silebilirsiniz. Silme işlemi geri alınamaz.

### Excel'de şifreleri görmek istemiyorum, nasıl gizlerim?
Excel export sırasında "Şifre sütununu dahil et" seçeneğini kaldırın.

### Raporlar başka bilgisayarda görünür mü?
Hayır, `reports.json` dosyasını kopyalamanız gerekir.

### Rapor yedekleri otomatik silinir mi?
Hayır, eski yedekler silinmez. Manuel temizleme yapmalısınız.

### PDF export'da logo nasıl eklerim?
PDF export sırasında "Logo Ekle" seçeneğinde logo dosyanızı seçin (PNG/JPG).

## 📚 İlgili Sayfalar

- [Arayüz Tanıtımı](interface.md)
- [Proje Yönetimi](projects.md)
- [Profil Backlink](profile-backlinks.md)
- [İpuçları ve Best Practices](../reference/best-practices.md)

---

**Önceki**: [Profil Backlink](profile-backlinks.md) | **Sonraki**: [Sık Sorulan Sorular](../reference/faq.md)
