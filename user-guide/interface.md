# interface

ProfyMob'un kullanıcı arayüzü modern ve kullanıcı dostu bir tasarıma sahiptir. Bu sayfa tüm arayüz öğelerini ve işlevlerini detaylı olarak açıklar.

## 📋 Ana Sayfa

Ana sayfa, yazılımın kontrol merkezi olarak görev yapar. Tüm önemli bilgilere ve ayarlara buradan erişebilirsiniz.

### Üst Panel

**Lisans Bilgileri**:

```
📋 Lisans Bilgileri
━━━━━━━━━━━━━━━━━━━━
Son Kullanma: 2025-12-31
Kalan Gün: 365 gün
Durum: ✅ Aktif
```

### Servis Ayarları Bölümü

#### Captcha Servisi

{% stepper %}
{% step %}
### Servis Seçimi

Dropdown menüden captcha servisinizi seçin:

* 2captcha.com
* anti-captcha.com
* capsolver.com
* capmonster.cloud
{% endstep %}

{% step %}
### API Key

Servis API anahtarınızı girin.
{% endstep %}

{% step %}
### Bakiye Kontrol

Mevcut bakiyenizi görüntüleyin:

* ✅ Yeşil: Yeterli bakiye
* ⚠️ Sarı: Düşük bakiye
* ❌ Kırmızı: Yetersiz bakiye
{% endstep %}
{% endstepper %}

#### Email Servisi

{% stepper %}
{% step %}
### Servis Seçimi

Dropdown menüden email servisinizi seçin:

* xmailhub.net (Önerilir)
* lution.ee
* zeus-x.ru
{% endstep %}

{% step %}
### API Key

Email servisi API anahtarınızı girin.
{% endstep %}

{% step %}
### Bakiye Kontrol

Email servisi bakiyenizi kontrol edin.
{% endstep %}
{% endstepper %}

### Proxy Ayarları

**Proxy Ekleme**:

* Manuel olarak tek proxy ekleme
* `proxies.txt` dosyası ile toplu ekleme

**Desteklenen Formatlar**:

```
ip:port
ip:port:username:password
http://ip:port
```

**Önerilen Proxy Servisleri**:

* [we1.town](https://we1.town/)
* [dataimpulse.com](https://dataimpulse.com/)
* [proxycin.com](https://proxycin.com/)

## 📁 Projeler Sayfası

Proje yönetim merkezi. Tüm projelerinizi buradan oluşturabilir ve yönetebilirsiniz.

### Proje Oluşturma

{% stepper %}
{% step %}
### Yeni Proje

"Yeni Proje" butonuna tıklayın.
{% endstep %}

{% step %}
### Proje Adı

Proje adı girin (örn: "Web Sitesi 1", "Müşteri X").
{% endstep %}

{% step %}
### Kaydet

"Kaydet" butonuna tıklayın.

Not: Diğer tüm bilgiler (kullanıcı adı, açıklama, linkler) ilgili backlink sayfalarında "Ayarları Kaydet" butonu ile projeye kaydedilir.
{% endstep %}
{% endstepper %}

### Proje İşlemleri

**Proje Seçme**:

* Listeden bir projeye tıklayarak seçin
* Seçili proje tüm backlink işlemlerinde kullanılır

**Proje Düzenleme**:

* Proje adını değiştirme
* Proje silme
* Kayıtlı ayarları görüntüleme

## 🎯 Backlink Sayfaları

ProfyMob 4 farklı backlink tipi için ayrı sayfalar sunar.

### Profil Backlink Sayfası

**Platform Seçimi**:

* Dropdown menüden 45+ platform arasından seçim
* Her platform için özel form alanları
* Platform durumu (Aktif/Bakımda)

**İşlem Bilgileri**:

* **Kullanıcı Adı**: Oluşturulacak profil için kullanıcı adı
* **Açıklama**: Profil bio/hakkında metni
* **Web Sitesi**: Backlink eklenecek URL
* **İşlem Sayısı**: Kaç tane profil oluşturulacağı (1-100)

**Ayarları Kaydet**:

* Girdiğiniz bilgileri projeye kaydedin
* Daha sonra tekrar kullanmak için

**Başlat Butonu**:

* İşlemi başlatır
* İşlem durumu gerçek zamanlı olarak gösterilir

### Sosyal Backlink Sayfası

**Platform Seçimi**:

* Sosyal işaretleme platformları
* Bookmark siteleri

**İşlem Bilgileri**:

* **Başlık**: Paylaşım başlığı
* **Açıklama**: Paylaşım açıklaması
* **URL**: Paylaşılacak link
* **Etiketler**: İlgili etiketler
* **İşlem Sayısı**: Kaç platform kullanılacağı

**Özellikler**:

* Hızlı işlem süresi
* Yüksek başarı oranı
* Hızlı indeksleme

### Web 2.0 Backlink Sayfası

**Platform Seçimi**:

* Blog platformları
* İçerik yayın siteleri

**İşlem Bilgileri**:

* **Kullanıcı Adı**: Blog hesabı kullanıcı adı
* **Blog Başlığı**: Yazı başlığı
* **Blog İçeriği**: Makale metni (minimum 300 kelime)
* **Web Sitesi**: Backlink URL
* **İşlem Sayısı**: Kaç blog yazısı

**İpucu**: İçeriğiniz ne kadar kaliteli olursa başarı oranı o kadar yüksek olur.

### Yorum Backlink Sayfası

**Link Dosyası**:

* WordPress blog URL'lerini içeren .txt dosyası
* Her satırda bir URL

**İşlem Bilgileri**:

* **Web Sitesi**: Backlink URL
* **Anahtar Kelime**: Anchor text
* **Yorum İçeriği**: Bırakılacak yorum metni
* **İşlem Sayısı**: Kaç yorumda link bırakılacağı

**Not**: Alakalı ve değerli yorumlar yazın, spam görünmeyin.

## 📊 Raporlar Sayfası

Oluşturduğunuz tüm backlink'lerin detaylı raporlarını görüntüleyin.

### Rapor Listesi

**Görüntülenen Bilgiler**:

* Platform adı
* Profile URL
* Email adresi
* Şifre
* Kullanıcı adı
* Oluşturulma tarihi
* Durum (✅ Başarılı / ❌ Başarısız)

### Filtreleme

**Filtre Seçenekleri**:

* Tarih aralığı
* Platform
* Proje
* Durum (Başarılı/Başarısız)

### Dışa Aktarma

**Excel Export**:

* Tüm rapor verilerini .xlsx formatında indirin
* Tüm alanlar dahil
* Tarih damgalı dosya adı

**PDF Export**:

* Profesyonel PDF raporu
* Müşteri sunumları için uygun
* Logo ve başlık bilgileri

### Rapor İşlemleri

**Tek Rapor Silme**:

* Seçili raporu sil

**Toplu Silme**:

* Birden fazla raporu seç ve sil
* Tarih aralığına göre toplu silme

**Yedekleme**:

* `reports.json` dosyasını manuel yedekleyin
* Düzenli yedekleme önerilir

## ⚙️ Ayarlar Sayfası

Genel yazılım ayarlarını yönetin.

### Genel Ayarlar

**Dil Seçimi**: Türkçe (varsayılan)

**Tema**:

* Açık tema (Gelecek güncellemede)
* Koyu tema

**Otomatik Güncelleme**:

* Yazılım başlangıcında güncelleme kontrolü
* Yeni sürüm bildirimi

### İşlem Ayarları

**Timeout Süreleri**:

* Email doğrulama timeout: 60 saniye (varsayılan)
* Captcha çözüm timeout: 120 saniye (varsayılan)
* Platform yanıt timeout: 30 saniye (varsayılan)

**Yeniden Deneme**:

* Başarısız işlemleri otomatik tekrar dene
* Maksimum deneme sayısı: 3

### Proxy Ayarları

**Proxy Kullanımı**:

* Tüm işlemlerde proxy kullan (Önerilir)
* Proxy rotation (Otomatik)

**Proxy Listesi**:

* Aktif proxy sayısı
* Proxy formatı kontrolü
* Geçersiz proxy'leri listele

### Bildirimler

**Ses Bildirimleri**:

* İşlem tamamlandığında ses bildirimi

**Masaüstü Bildirimleri**:

* Windows bildirim sistemi entegrasyonu

## 📈 İşlem Durumu Göstergeleri

### Gerçek Zamanlı Durum

1. 🔄 Başlatılıyor: İşlem hazırlanıyor
2. 🔄 Email Oluşturuluyor: Geçici email adresi alınıyor
3. 🔄 Hesap Kaydediliyor: Platform kayıt formu dolduruluyor
4. 🔄 Captcha Çözülüyor: Captcha servisi çalışıyor
5. 🔄 Email Doğrulanıyor: Doğrulama emaili bekleniyor
6. 🔄 Profil Düzenleniyor: Profil bilgileri ekleniyor
7. ✅ Tamamlandı: Backlink başarıyla oluşturuldu
8. ❌ Başarısız: Hata oluştu, detaylar gösteriliyor

### İlerleme Çubuğu

**Görsel Göstergeler**:

* Yüzde olarak ilerleme (0-100%)
* Tamamlanan/Toplam sayısı (örn: 5/10)
* Tahmini kalan süre

### Hata Bildirimleri

**Hata Türleri**:

* Captcha çözülemedi
* Email doğrulaması zaman aşımı
* Proxy bağlantı hatası
* Platform yanıt vermiyor
* Bakiye yetersiz

Her hata için:

* Açıklayıcı mesaj
* Çözüm önerisi
* Yeniden deneme seçeneği

## 🎨 Kısayol Tuşları

**Genel**:

* Ctrl + N: Yeni proje
* Ctrl + S: Ayarları kaydet
* Ctrl + R: Raporları görüntüle
* F5: Sayfayı yenile

**Proje Yönetimi**:

* Ctrl + D: Projeyi sil
* Ctrl + E: Projeyi düzenle

**İşlem Kontrolü**:

* Ctrl + Enter: İşlemi başlat
* Esc: İşlemi durdur

## 💡 Kullanım İpuçları

### Verimlilik

{% stepper %}
{% step %}
### Sık Kullanılan Ayarları Kaydedin

"Ayarları Kaydet" özelliğini kullanın.
{% endstep %}

{% step %}
### Proxy Listesi Hazırlayın

İşlem öncesi `proxies.txt` dosyasını doldurun.
{% endstep %}

{% step %}
### Toplu İşlemler

Birden fazla platformda aynı anda çalışın.
{% endstep %}

{% step %}
### Filtreleri Kullanın

Raporlarda filtreleme ile hızlıca bulun.
{% endstep %}
{% endstepper %}

### Organizasyon

{% stepper %}
{% step %}
### Proje İsimlendirme

Açıklayıcı isimler kullanın (örn: "Web1-Dev.to", "Müşteri2-Social").
{% endstep %}

{% step %}
### Düzenli Rapor Export

Haftada bir Excel raporu alın.
{% endstep %}

{% step %}
### Yedekleme

`config.json` ve `reports.json` dosyalarını yedekleyin.
{% endstep %}
{% endstepper %}

### Performans

{% stepper %}
{% step %}
### Proxy Kullanın

Toplu işlemlerde mutlaka proxy kullanın.
{% endstep %}

{% step %}
### Yavaş İlerleyin

Günlük 10-20 backlink yeterlidir.
{% endstep %}

{% step %}
### Bakiye Takibi

Servis bakiyelerinizi düzenli kontrol edin.
{% endstep %}

{% step %}
### Platform Çeşitliliği

Farklı platformlar kullanın.
{% endstep %}
{% endstepper %}

## ❓ Sık Sorulan Sorular

<details>

<summary>Arayüz donuyor mu?</summary>

Hayır, işlemler arka planda çalışır. İşlem devam ederken diğer sekmeleri kullanabilirsiniz.

</details>

<details>

<summary>Aynı anda birden fazla işlem çalıştırabilir miyim?</summary>

Hayır, aynı anda sadece bir işlem çalışabilir. İşlem bitince yeni işlem başlatabilirsiniz.

</details>

<details>

<summary>Ayarlarım kaydediliyor mu?</summary>

Evet, tüm ayarlar otomatik olarak `config.json` dosyasına kaydedilir.

</details>

<details>

<summary>Raporlar nerede saklanıyor?</summary>

`reports.json` dosyasında saklanır. Export ettiğiniz Excel/PDF dosyaları `reports/` klasöründe bulunur.

</details>

## 📚 İlgili Sayfalar

* [İlk Kullanım](/broken/pages/98bef36f5274dc74eec52967dcd0a42a8c8f0633)
* [Proje Yönetimi](/broken/pages/4a919aa9fad7d848c8cdcfcf57a3d2234859b3a4)
* [Profil Backlink](/broken/pages/7e5b0025e1b9e298c86b3622e8105d620237340e)
* [Raporlar](/broken/pages/ee4b4b029fd44da3ac42e309822a29716a956159)
