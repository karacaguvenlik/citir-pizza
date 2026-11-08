# Çıtır Pizza & Cafe — gösterim demosu

Yalnızca sunum amacıyla hazırlanmış statik sitedir. Türkçe, İngilizce, Almanca ve Rusça menü; ürün araması, kategori filtreleri, sepet ve bölge seçimi çalışır.

**Gerçek sipariş, ödeme, müşteri bilgisi toplama, yönetici girişi veya reklam ölçümü yoktur.** Fiyatlar örnektir. Sepet yalnızca ziyaretçinin kendi tarayıcısında saklanır.

## GitHub Pages yayını

1. Bu değişiklikleri `main` dalına birleştirin.
2. **Settings → Pages → Build and deployment → Source: Deploy from a branch** seçin.
3. **Branch: main**, klasör: **/(root)**, ardından **Save**.
4. Pages dağıtımı tamamlandığında site adresi: `https://karacaguvenlik.github.io/citir-pizza/`.

Bu adres dağıtım tamamlanmadan çalışmayabilir. Karaca Güvenlik sitesinin deposu veya ayarları değiştirilmez.

## Yerel kontrol

`python3 -m http.server 8000` çalıştırın ve tarayıcıda `http://localhost:8000` açın. Sunucu uygulaması veya gizli anahtar gerekmez.

Menü ve görseller işletme sahibinin sağladığı menüden aktarılmıştır; bazı ürünlerde temsili kategori görseli kullanılır. Gerçek fiyat, alerjen ve ticari bilgiler yayın öncesinde işletme tarafından doğrulanmalıdır.
