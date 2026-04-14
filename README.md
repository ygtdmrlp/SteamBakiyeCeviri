# Steam USD → TRY Fiyat Çevirici

Steam Store sayfasındaki **$** fiyatlarını canlı döviz kuruyla **₺** cinsine çeviren Chrome eklentisi.

---

## Ekran Görüntüleri

![Sayfa üzerindeki fiyat çevirisi](https://i.hizliresim.com/7dgtiyx.png)

![Popup paneli](https://i.hizliresim.com/9xrhwzr.png)

---

## Özellikler

- Steam Store'daki tüm USD fiyatlarını otomatik olarak TRY'ye çevirir
- Canlı döviz kuru çeker (saatte bir güncellenir, önbelleğe alınır)
- Sayfa üzerinde açma/kapama toggle paneli
- Popup üzerinden kur yenileme ve durum takibi
- Kur alınamazsa son geçerli önbellek değerini kullanır
- Shadow DOM ile sayfa tasarımına müdahale etmez

---

## Kurulum

1. Yeşil **Code** butonuna tıklayın → **Download ZIP** seçin ve ZIP'i bilgisayarınıza çıkartın.
2. Chrome'da adres çubuğuna `chrome://extensions` yazın ve Enter'a basın.
3. Sağ üst köşeden **Geliştirici modu**nu açın.
4. **Paketlenmemiş öğe yükle** butonuna tıklayın.
5. ZIP'ten çıkardığınız `steam-try-extension` klasörünü seçin.
6. Eklenti listeye eklenir, artık kullanıma hazır.

---

## Kullanım

1. [store.steampowered.com](https://store.steampowered.com) adresine gidin.
2. Sayfadaki tüm `$` fiyatları otomatik olarak `₺` karşılığıyla gösterilir.
3. Sağ üst köşedeki panelden çeviriyi açıp kapatabilirsiniz.
4. Toolbar'daki eklenti ikonuna tıklayarak kuru manuel olarak yenileyebilirsiniz.

---

## Döviz Kuru Kaynakları

Kur verisi sırasıyla şu API'lerden çekilir:

- [open.er-api.com](https://open.er-api.com)
- [exchangerate-api.com](https://www.exchangerate-api.com)

Her iki kaynak da başarısız olursa son önbellek değeri kullanılır.

---

## İzinler

| İzin | Neden |
|------|-------|
| `storage` | Kur ve ayarları önbelleğe almak için |
| `store.steampowered.com` | Fiyatları dönüştürmek için |
| `open.er-api.com` / `exchangerate-api.com` | Canlı kur çekmek için |

---

## Sürüm

`v1.0.0`

---

## Yapımcı

Yiğit
