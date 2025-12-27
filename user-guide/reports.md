# reports

ProfyMob, oluşturduğunuz tüm backlink'lerin detaylı raporlarını tutar. Raporları görüntüleyebilir, filtreleyebilir ve Excel/PDF formatında dışa aktarabilirsiniz.

## 📊 Rapor Sistemi

### Rapor Nedir?

Her başarılı backlink oluşturma işlemi için otomatik olarak bir rapor kaydı oluşturulur.

Rapor İçeriği:

* Profile/Hesap URL'si
* Email adresi
* Şifre
* Kullanıcı adı

### Raporlar Nasıl Saklanır?

Yerel Depolama:

* Tüm raporlar `reports.json` dosyasında saklanır
* Dosya yazılım klasöründe bulunur
* Otomatik olarak güncellenir
* Sadece bilgisayarınızda saklanır

Güvenlik:

* Şifreler düz metin olarak saklanır
* Dosyayı güvenli tutun
* Düzenli yedekleme yapın
* Paylaşmayın

## 📋 Raporlar Sayfası

### Ana Görünüm

Sol menüden **"Raporlar"** sekmesine tıklayarak raporlar sayfasına ulaşabilirsiniz.

Tablo Sütunları:

| Sütun         | Açıklama                  |
| ------------- | ------------------------- |
| Durum         | ✅ Başarılı / ❌ Başarısız  |
| Platform      | Platformun adı            |
| Profil URL    | Oluşturulan profil linki  |
| Email         | Kullanılan email adresi   |
| Şifre         | Hesap şifresi             |
| Kullanıcı Adı | Hesap kullanıcı adı       |
| Proje         | Hangi projede oluşturuldu |
| Tarih         | Oluşturulma tarihi        |
| Süre          | İşlem süresi (saniye)     |

### Rapor Detayları

Bir rapora tıklayarak detaylı bilgileri görüntüleyebilirsiniz:

Detay Penceresi:

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
Proxy: socks5://proxy.example.com:1080

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

Arama Çubuğu:

* Platform adıyla ara
* Email adresine göre ara
* Kullanıcı adına göre ara
* Proje adına göre ara
* URL'ye göre ara

Örnek Aramalar:

```
"dev.to" → Dev.to platformundaki tüm raporlar
"@example.com" → Belirli domain emaili içeren raporlar
"Müşteri1" → Belirli projede oluşturulan raporlar
"johndoe" → Kullanıcı adı içeren raporlar
```

### Gelişmiş Filtreler

#### Tarih Filtreleme

Ön Tanımlı Aralıklar:

* Bugün
* Dün
* Son 7 gün
* Son 30 gün
* Bu ay
* Geçen ay
* Tüm zamanlar

{% stepper %}
{% step %}
### Özel Tarih Aralığı

* "Özel Aralık" seçin
* Başlangıç tarihi seçin
* Bitiş tarihi seçin
* "Uygula" butonuna tıklayın
{% endstep %}
{% endstepper %}

#### Platform Filtreleme

Tek Platform:

* Dropdown menüden platform seçin
* Sadece o platformun raporları gösterilir

Çoklu Platform:

* Birden fazla platform seçin (Ctrl+tıklama)
* Seçili platformların raporları gösterilir

#### Proje Filtreleme

Tek Proje:

* Dropdown menüden proje seçin
* Sadece o projenin raporları gösterilir

Çoklu Proje:

* Birden fazla proje seçin
* Seçili projelerin raporları gösterilir

#### Durum Filtreleme

Filtre Seçenekleri:

* ✅ Sadece Başarılı
* ❌ Sadece Başarısız
* 🔄 Tümü

### Sıralama

Sıralama Seçenekleri:

* Tarihe göre (Yeni → Eski)
* Tarihe göre (Eski → Yeni)
* Platforma göre (A-Z)
* Platforma göre (Z-A)
* Projeye göre (A-Z)
* Duruma göre (Başarılı önce)

## 📤 Dışa Aktarma (Export)

### Excel Export

{% stepper %}
{% step %}
### Adımlar

* Export edilecek raporları filtreleyin (opsiyonel)
* **"Excel Export"** butonuna tıklayın
* Kaydetmek istediğiniz yeri seçin
* Dosya adı girin (varsayılan: `profymob_rapor_YYYYMMDD_HHMMSS.xlsx`)
* **"Kaydet"** butonuna tıklayın
{% endstep %}

{% step %}
### Excel İçeriği

* Tüm rapor alanları dahil
* Her satır bir backlink
* Başlık satırı dahil
* Filtreler uygulanmış
{% endstep %}

{% step %}
### Excel Sütunları

| Sütun | İçerik             |
| ----- | ------------------ |
| A     | Durum              |
| B     | Platform           |
| C     | Profil URL         |
| D     | Email              |
| E     | Şifre              |
| F     | Kullanıcı Adı      |
| G     | Proje              |
| H     | Oluşturulma Tarihi |
| I     | İşlem Süresi       |
{% endstep %}

{% step %}
### Kullanım Alanları

* Müşteri raporlama
* Backlink listeleme
* Veri analizi
* Yedekleme
{% endstep %}
{% endstepper %}

### PDF Export

{% stepper %}
{% step %}
### Adımlar

* Export edilecek raporları filtreleyin (opsiyonel)
* **"PDF Export"** butonuna tıklayın
* PDF ayarlarını yapın:
  * Logo ekle (opsiyonel)
  * Başlık metni
  * Alt bilgi
* **"Oluştur"** butonuna tıklayın
* Kaydetmek istediğiniz yeri seçin
{% endstep %}

{% step %}
### PDF İçeriği

* Profesyonel tasarım
* Logo ve başlık
* Tablo formatında raporlar
* Sayfa numaraları
* Oluşturulma tarihi
* Toplam istatistikler
{% endstep %}

{% step %}
### Kullanım Alanları

* Müşteri sunumları
* Profesyonel raporlar
* Yazdırma
* Arşivleme
{% endstep %}
{% endstepper %}

### CSV Export

{% stepper %}
{% step %}
### Adımlar

* Export edilecek raporları filtreleyin (opsiyonel)
* **"CSV Export"** butonuna tıklayın
* Ayırıcı seçin (virgül, noktalı virgül, tab)
* Kaydetmek istediğiniz yeri seçin
* **"Kaydet"** butonuna tıklayın
{% endstep %}

{% step %}
### CSV İçeriği

* Basit metin formatı
* Excel'de açılabilir
* Veritabanına import edilebilir
{% endstep %}

{% step %}
### Kullanım Alanları

* Veri taşıma
* Diğer yazılımlara import
* Veritabanı entegrasyonu
{% endstep %}
{% endstepper %}

## 🗑️ Rapor Yönetimi

### Tek Rapor Silme

{% stepper %}
{% step %}
* Silinecek rapora tıklayın
* **"Sil"** butonuna tıklayın
* Onay mesajı: "Bu rapor silinecek, emin misiniz?"
* **"Evet, Sil"** butonuna tıklayın
{% endstep %}

{% step %}
Uyarı:

* Silinen rapor geri alınamaz
* Excel/PDF export'u yoksa veri kaybolur
* Dikkatli olun
{% endstep %}
{% endstepper %}

### Toplu Silme

Seçerek Silme:

{% stepper %}
{% step %}
* Silinecek raporları seçin (Ctrl+tıklama veya Shift+tıklama)
* **"Seçilenleri Sil"** butonuna tıklayın
* Onay mesajı: "X adet rapor silinecek, emin misiniz?"
* **"Evet, Sil"** butonuna tıklayın
{% endstep %}

{% step %}
Filtre ile Silme:

* Filtre uygulayın (örn: 30 günden eski raporlar)
* **"Filtrelileri Sil"** butonuna tıklayın
* Onay mesajı görünür
* **"Evet, Sil"** butonuna tıklayın
{% endstep %}

{% step %}
Tümünü Silme:

* **"Tüm Raporları Sil"** butonuna tıklayın
* Onay mesajı: "TÜM RAPORLAR SİLİNECEK! Emin misiniz?"
* Güvenlik sorusu: "Silmek için 'SIFIRLA' yazın"
* "SIFIRLA" yazıp **"Onayla"** butonuna tıklayın

Uyarı: Bu işlem geri alınamaz!
{% endstep %}
{% endstepper %}

### Rapor Düzenleme

Düzenlenebilir Alanlar:

* Notlar ekleyebilirsiniz
* Proje adını değiştirebilirsiniz
* Durum etiketleri ekleyebilirsiniz

Düzenlenemeyen Alanlar:

* Platform
* URL
* Email
* Şifre
* Tarih
* İşlem süresi

{% stepper %}
{% step %}
### Düzenleme Adımları

* Rapora tıklayın
* **"Düzenle"** butonuna tıklayın
* Değiştirmek istediğiniz alanları düzenleyin
* **"Kaydet"** butonuna tıklayın
{% endstep %}
{% endstepper %}

## 📈 Rapor İstatistikleri

### Genel İstatistikler

Raporlar sayfasının üst kısmında genel istatistikler görüntülenir:

Göstergeler:

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

{% stepper %}
{% step %}
### Görüntüleme

* **"Platform İstatistikleri"** butonuna tıklayın
* Platform listesi görünür
{% endstep %}

{% step %}
### İçerik

| Platform      | Toplam | Başarılı | Başarı Oranı | Ort. Süre |
| ------------- | ------ | -------- | ------------ | --------- |
| Dev.to        | 89     | 86       | 96.6%        | 95 sn     |
| WordPress.org | 67     | 66       | 98.5%        | 110 sn    |
| Pinterest.com | 54     | 48       | 88.9%        | 85 sn     |
| Disqus.com    | 43     | 42       | 97.7%        | 78 sn     |
{% endstep %}

{% step %}
### Grafikler

* Pasta grafiği: Platform dağılımı
* Çubuk grafiği: Başarı oranları
* Çizgi grafiği: Zaman içinde trend
{% endstep %}
{% endstepper %}

### Proje Bazında İstatistikler

{% stepper %}
{% step %}
### Görüntüleme

* **"Proje İstatistikleri"** butonuna tıklayın
* Proje listesi görünür
{% endstep %}

{% step %}
### İçerik

| Proje    | Toplam | Platform Sayısı | Başarı Oranı | İlk İşlem  | Son İşlem  |
| -------- | ------ | --------------- | ------------ | ---------- | ---------- |
| Müşteri1 | 156    | 12              | 94%          | 01.11.2024 | 27.12.2025 |
| Web1     | 89     | 8               | 91%          | 15.11.2024 | 25.12.2025 |
| Test     | 23     | 5               | 78%          | 20.12.2024 | 27.12.2025 |
{% endstep %}
{% endstepper %}

### Zaman Bazında Analiz

Görsel Gösterim:

* Günlük backlink sayısı (son 30 gün)
* Haftalık trend
* Aylık karşılaştırma
* Başarı oranı trendi

Örnek Grafik Verisi:

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

{% stepper %}
{% step %}
* ProfyMob klasörünü açın
* `reports.json` dosyasını bulun
* Dosyayı kopyalayın
* Güvenli bir yere kaydedin (cloud, USB vb.)
{% endstep %}

{% step %}
Önerilen Yedekleme Sıklığı:

* Günlük: Çok aktif kullanıyorsanız
* Haftalık: Normal kullanım
* Aylık: Az kullanım
{% endstep %}

{% step %}
Yedekleme İsimlendirmesi (örnekler):

```
reports_20251227.json
reports_backup_27_12_2025.json
profymob_reports_2025_12_27.json
```
{% endstep %}
{% endstepper %}

### Otomatik Yedekleme

{% stepper %}
{% step %}
### Ayarlama

* Ayarlar > Yedekleme sekmesine gidin
* **"Otomatik Yedekleme"** seçeneğini aktif edin
* Yedekleme sıklığını seçin (Günlük/Haftalık/Aylık)
* Yedekleme klasörünü seçin
* **"Kaydet"**
{% endstep %}

{% step %}
Otomatik Yedek Dosyaları (örnek):

```
backups/
├── reports_2025_12_27.json
├── reports_2025_12_20.json
├── reports_2025_12_13.json
└── reports_2025_12_06.json
```
{% endstep %}
{% endstepper %}

### Geri Yükleme

{% stepper %}
{% step %}
### Manuel Geri Yükleme

* ProfyMob'u kapatın
* Yedek `reports.json` dosyasını kopyalayın
* Mevcut `reports.json` dosyasının yerine yapıştırın
* ProfyMob'u başlatın
{% endstep %}

{% step %}
### Yazılım İçinden Geri Yükleme

* Ayarlar > Yedekleme > **"Geri Yükle"** butonuna tıklayın
* Yedek dosyayı seçin
* Geri yükleme seçeneği seçin:
  * **"Üzerine Yaz"**: Mevcut raporlar silinir, yedek yüklenir
  * **"Birleştir"**: Yedek raporlar mevcut raporlara eklenir
* **"Geri Yükle"** butonuna tıklayın

Uyarı: "Üzerine Yaz" seçeneği mevcut raporları siler!
{% endstep %}
{% endstepper %}

## 🔒 Güvenlik ve Gizlilik

### Şifre Güvenliği

Raporlarda Şifreler:

* ❌ Şifrelenmiş DEĞİL
* ✅ Düz metin olarak saklanır
* ⚠️ Güvenli tutun

Öneriler:

1. `reports.json` dosyasını kimseyle paylaşmayın
2. Cloud yedekleme yapıyorsanız şifreli cloud kullanın
3. Bilgisayarınızı şifre ile koruyun
4. Güvenli yerden çalışın

### Veri Gizliliği

Yerel Depolama:

* Tüm raporlar sadece bilgisayarınızda
* Sunucuya gönderilmez
* İnternet gerektirmez (görüntüleme için)

Export Güvenliği:

* Excel/PDF dosyaları şifre korumalı yapılabilir
* Hassas bilgiler içerebilir
* Dikkatli paylaşın

## 💡 İpuçları ve Best Practices

### Organizasyon

1. Düzenli Export: Haftada bir Excel raporu alın
2. Eski Raporları Temizleyin: 6 ay önceki raporları silin
3. Proje Bazlı Takip: Her proje için ayrı rapor tutun
4. Notlar Ekleyin: Önemli backlinklere not ekleyin

### Analiz

1. Başarı Oranını Takip Edin: Platform başına başarı oranı
2. En İyi Platformları Belirleyin: Yüksek başarı oranına odaklanın
3. Trend Analizi: Zaman içinde backlink artışı
4. Başarısızlık Sebeplerini Inceleyin: Hangi platformlarda sorun var?

### Yedekleme

1. Otomatik Yedekleme Kurun: Veri kaybını önler
2. Cloud Yedekleme: Dropbox, Google Drive gibi
3. Versiyonlama: Eski yedekleri sakla
4. Test Edin: Geri yüklemenin çalıştığını test edin

### Performans

1. Eski Raporları Arşivleyin: Yazılım hızını artırır
2. Filtreleri Kullanın: Büyük listelerde arama yapın
3. Excel Export: Büyük analizler için Excel kullanın

## ❓ Sık Sorulan Sorular

<details>

<summary>Kaç rapor saklayabilirim?</summary>

Sınır yok, ancak 10,000+ raporda performans düşebilir. Eski raporları arşivleyin.

</details>

<details>

<summary>Raporları silebilir miyim?</summary>

Evet, tek tek veya toplu olarak silebilirsiniz. Silme işlemi geri alınamaz.

</details>

<details>

<summary>Excel'de şifreleri görmek istemiyorum, nasıl gizlerim?</summary>

Excel export sırasında "Şifre sütununu dahil et" seçeneğini kaldırın.

</details>

<details>

<summary>Raporlar başka bilgisayarda görünür mü?</summary>

Hayır, \`reports.json\` dosyasını kopyalamanız gerekir.

</details>

<details>

<summary>Rapor yedekleri otomatik silinir mi?</summary>

Hayır, eski yedekler silinmez. Manuel temizleme yapmalısınız.

</details>

<details>

<summary>PDF export'da logo nasıl eklerim?</summary>

PDF export sırasında "Logo Ekle" seçeneğinde logo dosyanızı seçin (PNG/JPG).

</details>

## 📚 İlgili Sayfalar

* [Arayüz Tanıtımı](/broken/pages/ea4eef21db85191c84d2fc0d2a2722dbd7e9f9d0)
* [Proje Yönetimi](/broken/pages/4a919aa9fad7d848c8cdcfcf57a3d2234859b3a4)
* [Profil Backlink](/broken/pages/7e5b0025e1b9e298c86b3622e8105d620237340e)
* [İpuçları ve Best Practices](/broken/pages/2eee74b3117a73768adc5032f852b15bde26c530)
