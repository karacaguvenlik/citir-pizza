# Çıtır Pizza & Cafe — tam gösterim demosu

GitHub Pages üzerinde çalışan müşteri sitesi ve **temsili yönetim paneli**.

- Site: https://karacaguvenlik.github.io/citir-pizza/
- Demo paneli: https://karacaguvenlik.github.io/citir-pizza/admin.html
- Panele **Demoyu aç** ile girilir. Parola veya gerçek kullanıcı yetkilendirmesi yoktur.

## Neler denenebilir?

Dört dil (TR/EN/DE/RU), menü araması, kategoriler, sepet, bölge minimumu ve temsili sipariş oluşturma. Aynı tarayıcıda oluşturulan örnek sipariş panelde görünür. Ürün/fiyat, kategori, teslimat bölgesi ve site metinleri panelden değiştirilebilir. Demo sıfırlama başlangıç verilerini geri getirir.

**Gerçek sipariş, tahsilat, müşteri bilgisi toplama veya güvenli admin girişi yoktur.** Kullanıcılar bölümü yalnızca temsili bilgilendirmedir. Online ödeme ve reklam ölçümü kapalıdır. Gerçek müşteri, personel veya kart bilgisi yazmayın.

Veriler `citir-presentation-v1` anahtarıyla ziyaretçinin tarayıcısında saklanır. Sepet/bölge tercihleri de demo adına ayrılmış anahtarlardadır. Diğer cihazlar veya farklı tarayıcılar değişiklikleri görmez; ortak sunucu veritabanı yoktur. Bu durum demo uyarılarında açıkça belirtilir. Fiyatlar örnektir.

## GitHub Pages

Settings → Pages → Deploy from a branch → **main / (root)**. Bu depoda ayar zaten yapılmışsa, değişiklikler main dalına birleştirildiğinde Pages yayını güncellenir. Dağıtım tamamlanana kadar eski sürüm görünebilir.

## Yerel kontrol

Node.js 24+: `node --test tests/presentation.test.mjs`.
Statik dosyaları incelemek için `python3 -m http.server 8000`, ardından `http://localhost:8000`.

Dosya yolları görecelidir; `/citir-pizza/` veya başka alt klasörde yayınlanabilir. Dış fontlar için Google Fonts bağlantısı vardır; reklam etiketi yoktur. `noindex` yalnızca indekslemeyi engelleme talebidir, erişim kontrolü değildir.

## Depodaki ayrı sunuculu sürüm

Önceden mevcut `server.py` ve `static/` dosyaları bu değişiklikte korunmuştur. Bunlar GitHub Pages tarafından çalıştırılmaz ve buradaki temsili panelden ayrıdır. GitHub yayını için herhangi bir sunucu uygulaması başlatmayın; bu sunucu sürümü burada üretime hazır olarak değerlendirilmemiştir.
