# Pinterest Media Analyzer (Pinterest Medya Analiz Aracı)

> 🔍 Eğitim ve araştırma amaçlı geliştirilmiş, Pinterest'teki herkese açık içeriklerden meta veri çıkarmayı destekleyen hafif bir ön uç aracı

🌐 Canlı Demo: [https://twittervideodownloaderx.com/pinterest_downloader_tu](https://twittervideodownloaderx.com/pinterest_downloader_tu)

---

## 📋 Proje Genel Bakış

Bu proje, eğitim ve teknik araştırma amaçlarıyla geliştirilmiştir. Geliştiricilerin ve öğrencilerin, OEmbed gibi standart web API'lerini kullanarak herkese açık Pinterest sayfalarından yapılandırılmış meta verileri (Schema.org ve Open Graph etiketleri gibi) nasıl çıkarabileceklerini anlamalarına yardımcı olmak için tasarlanmış hafif bir ön uç yardımcı programıdır.

> 🎯 Önerilen Kullanım Senaryoları:
> - Kişisel çalışma materyallerinin düzenlenmesi ve fikir toplama
> - Ön uç geliştirme pratiği ve web veri çıkarma araştırmaları
> - Multimedya meta veri yapıları hakkında öğrenme
> - Telif hakkı sahiplerinden açık izin alınmış içeriğin arşivlenmesi

⚠️ **Önemli Uyarı**: Bu araç yalnızca **herkese açık erişilebilir içeriklerle** çalışır. Giriş gerektiren, ücretli veya özel olarak ayarlanmış Pinterest içeriklerine erişim sağlamak için tasarlanmamıştır ve bu amaçla kullanılmamalıdır.

---

## ✨ Temel Özellikler

- 🔗 **Akıllı Bağlantı Tanıma**: Pinterest Pin URL'lerini, kısa bağlantıları ve mobil formatlı bağlantıları otomatik olarak algılar
- 🎬 **Çoklu Format Desteği**: MP4 videolar, WebM animasyonlar, JPG/PNG görseller ve diğer yaygın medya formatları için meta veri çıkarır
- 📐 **Çözünürlük Bilgisi Gösterimi**: Kullanılabilir çözünürlük seçeneklerini ve dosya formatlarını bilinçli seçim için görüntüler
- 📱 **Tamamen Duyarlı Tasarım**: Masaüstü, tablet ve mobil cihazlarda optimize edilmiş kullanıcı deneyimi
- ⚡ **İstemci Tarafı Öncelikli Mimari**: Temel analiz mantığı tarayıcıda çalışır, sunucu bağımlılığını azaltır ve yanıt süresini iyileştirir
- 🔐 **Gizliliğe Saygılı Tasarım**: Gönderilen URL'leri kaydetmez, analiz sonuçlarını depolamaz veya herhangi bir kişisel kullanıcı verisi toplamaz

---

## 🚀 Hızlı Başlangıç Kılavuzu

1. Pinterest uygulamasını veya web sitesini açın ve başvurmak istediğiniz **herkese açık içeriği** bulun
2. Tarayıcınızın adres çubuğundan sayfa URL'sini kopyalayın (örnek: `https://www.pinterest.com/pin/1234567890/`)
3. Bağlantıyı bu aracın giriş alanına yapıştırın ve "Analiz Et" düğmesine tıklayın
4. Sistem, herkese açık meta verileri çıkaracak ve erişilebilir kaynak bilgilerini görüntüleyecektir
5. Tercih ettiğiniz formatı/çözünürlüğü seçin, ardından bağlantıya sağ tıklayıp "Farklı kaydet..." seçeneğini seçerek yerel olarak indirin

> 💡 Kullanım İpuçları:
> - Hedef içeriğin "Herkese Açık" görünürlük ayarında olduğundan her zaman emin olun
> - Analiz başarısız olursa, sayfayı yenilemeyi veya ağ bağlantınızı kontrol etmeyi deneyin
> - Öğrenme amaçlı olarak, bu araçla birlikte tarayıcı Geliştirici Araçlarını (F12 → Network → Fetch/XHR) kullanmayı düşünün

---

## ⚠️ Uyumluluk ve Sorumluluk Reddi (Lütfen Dikkatlice Okuyun)

Bu proje, "teknik tarafsızlık" ve "yasal uyumluluk" ilkeleri çerçevesinde faaliyet göstermektedir. Kullanmadan önce lütfen aşağıdakileri inceleyin ve kabul edin:

### ✅ Önerilen Uygulamalar
- Yalnızca yasal erişim hakkınız olan **herkese açık içerikleri** analiz edin
- Çıkarılan kaynakları yalnızca **kişisel öğrenme, araştırma veya özel referans** amacıyla kullanın
- Yeniden dağıtım, türev eser oluşturma veya ticari kullanım előtt telif hakkı sahiplerinden açık yazılı izin alın
- Projelerinizde her zaman orijinal yaratıcıları belirtin ve kaynak atıfını açıkça gösterin

### ❌ Yasaklanan Eylemler
- Giriş gerektiren, ücretli veya özel olarak ayarlanmış içeriğe erişmeye veya analiz etmeye çalışmak
- Bu aracı ticari kazıma, veri toplama hizmetleri veya reklam geliri elde etmek için kullanmak
- Yüksek frekanslı otomatik istekler, bot trafiği veya Pinterest hizmetlerini aksatabilecek herhangi bir etkinlik göndermek
- Filigranları, telif hakkı bildirimlerini veya gömülü meta verileri kaldırmak, değiştirmek veya gizlemek

> 📜 Yasal Uyarı:
> Bu aracın kullanımı, geçerli telif hakkı yasalarına (DMCA, AB Telif Hakkı Direktifi ve yerel düzenlemeler dahil ancak bunlarla sınırlı olmamak üzere) ve Pinterest'in [Topluluk Kuralları](https://policy.pinterest.com/community-guidelines) ile [Geliştirici Politikası](https://developers.pinterest.com/docs/api/policy/)'na uygun olmalıdır.
> Geliştiriciler, son kullanıcılar tarafından bu aracın kötüye kullanımından kaynaklanan herhangi bir yasal sorun, zarar veya kayıptan sorumlu değildir.

---

## 🛠 Teknik Uygulama Notları (Geliştiriciler İçin)

> Genel kullanıcılar bu bölümü atlayabilir

### Mimari Genel Bakış
```
Kullanıcı Tarayıcısı → İstemci Tarafı Analiz Modülü → Pinterest Genel Uç Noktaları / OEmbed → Yapılandırılmış Veri Çıkarma → Sonuç İşleme
```

### Temel Teknik Yaklaşımlar
- Genel sayfa meta verilerini almak için uygun CORS proxy yapılandırması ile `fetch` API'sini kullanır
- `<script type="application/ld+json">` etiketlerinden Schema.org yapılandırılmış verilerini ayrıştırır
- Kaynak keşfi için Open Graph meta verilerini (`og:video`, `og:image`, `og:title` vb.) kullanır
- Sağlam bağlantı tanıma için regex kalıpları + DOM ayrıştırma ile çift doğrulama uygular

### Kendi Sunucunuzda Barındırma Kılavuzu (Referans)
```bash
# 1. Depoyu klonlayın (örnek)
git clone https://github.com/yourname/pinterest-downloader-tu.git

# 2. Statik dosyaları dağıtın (HTTPS şiddetle önerilir)
#    - Vercel / Netlify / Cloudflare Pages (kolay kurulum, önerilir)
#    - Nginx + Let's Encrypt sertifikası (kendi kendine barındırma seçeneği)

# 3. Güvenlik başlıkları yapılandırma örneği (Nginx)
add_header Content-Security-Policy "default-src 'self'; script-src 'self' 'unsafe-inline';";
add_header X-Content-Type-Options "nosniff";
add_header Referrer-Policy "strict-origin-when-cross-origin";
add_header X-Frame-Options "DENY";
```

> 🔐 Üretim Ortamı Dağıtımı İçin En İyi Uygulamalar:
> - Ortadaki adam saldırılarını önlemek için her zaman HTTPS'yi etkinleştirin
> - Kötüye kullanımı ve aşırı istekleri önlemek için hız sınırlama (rate limiting) uygulayın
> - Kötüye kullanılabilecek hassas analiz mantığını ifşa etmekten kaçının
> - Güvenlik yamalarını uygulamak için bağımlılıkları düzenli olarak gözden geçirin ve güncelleyin

---

## 🤝 Katkıda Bulunma

Bu eğitim projesini geliştirmeye yardımcı olmak için topluluk katkılarını memnuniyetle karşılıyoruz!

| Katkı Türü | Örnekler |
|-----------|----------|
| 🐛 Hata Bildirimleri | Ayrıntılı adımlarla Sorun oluşturun: URL + tarayıcı bilgisi + yeniden üretim adımları |
| 💡 Özellik Önerileri | UX iyileştirmeleri, erişilebilirlik veya yeni eğitim özellikleri için yapıcı fikirler paylaşın |
| 🌍 Çeviri Yardımı | Arayüz metninin ek dillere çevrilmesine yardımcı olun |
| 📚 Dokümantasyon | Kullanım örnekleri, teknik diyagramlar veya uyumluluk kılavuzları ekleyin |

> Bu proje [MIT Lisansı](./LICENSE) altında yayınlanmaktadır. Eğitim ve araştırma amaçları için özgürce kullanım ve değişikliği teşvik ediyoruz. Ticari özelleştirme talepleri için lütfen ayrı kanallar üzerinden bizimle iletişime geçin.

---

## ❓ Sıkça Sorulan Sorular (SSS)

**S: "İçerik alınamadı" mesajı neden görünüyor?**  
C: Olası nedenler: ① Bağlantı özel/silinmiş içeriği işaret ediyor ② Pinterest sayfa yapısını geçici olarak değiştirdi ③ Ağ kısıtlamaları veya CORS sorunları. Çözüm: Genel durumu doğrulayın → Farklı bir ağda deneyin → Bekleyip tekrar deneyin.

**S: İndirilen videoda filigran var mı?**  
C: Bu araç, Pinterest'in resmi altyapısı tarafından sağlanan orijinal kaynak URL'lerini döndürür. Filigran varlığı tamamen içeriği yükleyen kullanıcının ayarlarına bağlıdır. Bu araç herhangi bir filigran veya gömülü işaret eklemez, kaldırmaz veya değiştirmez.

**S: Albümler veya Panolar için toplu işleme destekleniyor mu?**  
C: Mevcut sürüm, kararlılık ve uyumluluğu önceliklendirmek için tek Pin analizine odaklanmaktadır. Toplu işlemler için, lütfen önce kullanım durumunuzun Pinterest'in [Geliştirici Politikası](https://developers.pinterest.com/docs/api/policy/) ile hız sınırları ve veri kullanımı konusunda uyumlu olduğundan emin olun.

**S: Bu araç kullanım verilerimi veya kişisel bilgilerimi topluyor mu?**  
C: Hayır. Bu, arka uç günlüğü, analiz komut dosyaları veya çerez tabanlı izleme içermeyen tamamen statik bir ön uç projesidir. Tüm işleme, tarayıcı oturumunuz içinde yerel olarak gerçekleşir.

---

## 🌱 Felsefemiz

> Teknolojinin kendisi nötrdür. Önemli olan, onu kullananların *niyeti* ve *sorumluluğudur*.

Geliştiricileri ve kullanıcıları bu değerleri benimsemeye davet ediyoruz:

- 🔬 Merak ve etik öğrenme yoluyla web teknolojilerini daha derinlemesine anlamaya çalışmak
- 🤲 Kaynakları doğru şekilde belirterek ve izin alarak yaratıcıların haklarına saygı göstermek
- 🌍 İnovasyon ile kültürel mirasın korunması arasında denge kuran sağlıklı bir dijital ekosisteme katkıda bulunmak

Birlikte, yaratıcılık, paylaşım ve teknolojinin sorumlu kullanımının olumlu bir döngüsünü teşvik edelim ✨

---

## 📄 Lisans

Bu proje [MIT Lisansı](./LICENSE) altında dağıtılmaktadır.

```


Bu yazılımın ve ilişkili belgelendirme dosyalarının ("Yazılım") bir kopyasını
elde eden herhangi bir kişiye, aşağıdaki koşullar altında, Yazılımı
kullanma, kopyalama, değiştirme, birleştirme, yayınlama, dağıtma,
alt lisanslama ve/veya satma hakları ücretsiz olarak verilir:

Yukarıdaki telif hakkı bildirimi ve bu izin bildirimi, Yazılımın tüm
kopyalarında veya önemli bölümlerinde yer almalıdır.

YAZILIM "OLDUĞU GİBİ" SUNULMAKTADIR, AÇIK VEYA ZIMNİ OLARAK,
TİCARİ OLABİLİRLİK, BELİRLİ BİR AMACA UYGUNLUK VE İHLAL ETMEME
GARANTİLERİ DAHİL ANCAK BUNLARLA SINIRLI OLMAMAK ÜZERE HERHANGİ BİR
GARANTİ İÇERMEZ. HİÇBİR DURUMDA YAZARLAR VEYA TELİF HAKKI SAHİPLERİ,
SÖZLEŞME, HAKSIZ FİİL VEYA BAŞKA BİR ŞEKİLDE, YAZILIMDAN VEYA
YAZILIMIN KULLANIMINDAN VEYA YAZILIMLA İLGİLİ DİĞER İŞLEMLERDEN
KAYNAKLANAN HERHANGİ BİR TALEP, ZARAR VEYA DİĞER SORUMLULUKTAN
SORUMLU OLMAYACAKTIR.
```

---


*🔖 Sürüm: v1.2.0-tr (Ön uç optimizasyonu / Geliştirilmiş i18n desteği / Güçlendirilmiş uyumluluk dokümantasyonu)*