# 🔖 Sosyal İşaretleme

Sosyal işaretleme modülü, çeşitli sosyal işaretleme platformlarında otomatik olarak içerik paylaşmanızı sağlar. Bu özellik, web sitenize backlink oluşturmak ve SEO performansınızı artırmak için kullanılır.

## Genel Bakış

Sosyal işaretleme işlemi, belirlediğiniz platformlarda otomatik hesap oluşturma ve içerik paylaşma sürecidir. Sistem, captcha çözümü ve mail doğrulama ile tam otomatik çalışır.

## Özellikler

- ✅ Çoklu platform desteği
- ✅ Otomatik hesap oluşturma
- ✅ Captcha çözümü desteği
- ✅ Mail doğrulama desteği
- ✅ Proxy desteği
- ✅ Toplu işlem yapabilme
- ✅ Detaylı raporlama

## Kullanım Adımları

### 1. Proje Seçimi

İlk olarak bir proje seçmeniz gerekmektedir. Sosyal işaretleme işlemleri seçili projeye kaydedilecektir.

### 2. Platform Seçimi

Sosyal işaretleme yapmak istediğiniz platformu seçin:

- **Hepsi**: Tüm desteklenen platformlarda işlem yapar
- **Tek Platform**: Belirli bir platformda işlem yapar

### 3. Form Doldurma

Aşağıdaki bilgileri doldurun:

#### Kullanıcı Adı
- Oluşturulacak hesaplar için kullanılacak temel kullanıcı adı
- Sistem otomatik olarak her hesap için benzersiz bir kullanıcı adı oluşturur

#### Başlık
- Paylaşılacak içeriğin başlığı
- SEO dostu ve çekici bir başlık kullanın

#### İçerik
- Paylaşılacak içeriğin detayı
- İçeriğinizde web sitenizin linkini ekleyin
- Minimum 50, maksimum 500 karakter önerilir

#### Tekrar Sayısı
- Her platform için kaç kez işlem yapılacağını belirler
- Örnek: 5 giriş yaparsanız, her platformda 5 ayrı hesap oluşturulup içerik paylaşılır

### 4. Servis Gereksinimleri

Sosyal işaretleme işlemi için aşağıdaki servislerin yapılandırılmış olması **zorunludur**:

#### Captcha Servisi
- Ayarlar bölümünden bir captcha servisi seçin
- API anahtarınızı girin
- Servis bakiyenizi kontrol edin

Desteklenen servisler:
- 2Captcha
- Anti-Captcha
- CapSolver
- CapMonster

#### Mail Servisi
- Ayarlar bölümünden bir mail servisi seçin
- API anahtarınızı girin
- Servis bakiyenizi kontrol edin

Desteklenen servisler:
- Temp-Mail.org
- Guerrilla Mail
- Mail.tm

### 5. İşlemi Başlatma

"Başlat" butonuna tıklayarak işlemi başlatın. İşlem sırasında:

- Her platform için otomatik hesap oluşturulur
- Gerekli doğrulamalar yapılır
- İçerik paylaşılır
- Sonuçlar raporlanır

### 6. İşlemi Durdurma

İşlemi herhangi bir anda "Durdur" butonuna tıklayarak durdurabilirsiniz.

## Raporlama

İşlem tamamlandıktan sonra:

- Başarılı paylaşımlar raporlara kaydedilir
- Her paylaşım için URL bilgisi saklanır
- Proje istatistiklerine başarı/başarısızlık puanı eklenir
- Raporlar sekmesinden detayları görüntüleyebilirsiniz

## Önemli Notlar

### ⚠️ Gereksinimler

1. **Proje Seçimi**: İşlem başlatmadan önce mutlaka bir proje seçin
2. **Captcha Servisi**: Zorunlu - API anahtarı ve bakiye gerekli
3. **Mail Servisi**: Zorunlu - API anahtarı ve bakiye gerekli
4. **İnternet Bağlantısı**: Stabil bir bağlantı önerilir

### 💡 İpuçları

- İlk başta düşük tekrar sayısı ile test edin
- İçeriğinizi her platform için optimize edin
- Farklı zamanlarda işlem yaparak doğal görünün
- Proxy kullanımı IP engellemelerini önler
- Raporları düzenli olarak kontrol edin

### 🎯 En İyi Uygulamalar

1. **Kaliteli İçerik**: Spam olarak algılanmamak için kaliteli içerik paylaşın
2. **Doğal Hız**: Çok hızlı işlem yapmaktan kaçının
3. **Çeşitlilik**: Farklı platformları kullanın
4. **Takip**: Oluşturulan linkleri düzenli kontrol edin
5. **Denge**: Her gün makul sayıda backlink oluşturun

## Sorun Giderme

### İşlem Başlamıyor

- Proje seçili olduğundan emin olun
- Tüm form alanlarının dolu olduğunu kontrol edin
- Captcha ve mail servisi ayarlarını kontrol edin
- Servis bakiyelerini kontrol edin

### Başarısız İşlemler

- İnternet bağlantınızı kontrol edin
- Proxy ayarlarınızı gözden geçirin
- Captcha ve mail servis API anahtarlarını doğrulayın
- Platform geçici olarak erişilemez olabilir

### Düşük Başarı Oranı

- İçerik kalitesini artırın
- Farklı kullanıcı adları deneyin
- Proxy kullanın veya farklı proxy'ler deneyin
- İşlem hızını azaltın

## Teknik Detaylar

### Desteklenen Platformlar

Sistem, plugins/sites/ klasöründe tanımlı tüm sosyal işaretleme platformlarını destekler. Her platform için özel entegrasyon mevcuttur.

### Güvenlik

- Tüm işlemler şifreli bağlantı üzerinden yapılır
- Oluşturulan hesap bilgileri güvenli şekilde saklanır
- Proxy kullanımı ile IP gizliliği sağlanır

### Performans

- Çoklu thread desteği ile hızlı işlem
- Timeout koruması
- Otomatik hata yakalama ve devam etme

## Sonraki Adımlar

- [Web 2.0 Blog Yazıları](web20-blogs.md) - Web 2.0 platformlarında blog yazısı oluşturma
- [WordPress Yorum](wordpress-comments.md) - WordPress sitelerine yorum yapma
- [Forum İşlemleri](forum-operations.md) - Forum sitelerinde profil ve içerik oluşturma
- [Raporlar](reports.md) - İşlem sonuçlarını görüntüleme
