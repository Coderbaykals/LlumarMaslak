# Galeri Görselleri

Bu klasöre yüklenen JPG dosyaları, `index.html` içindeki galeri kartlarında otomatik gösterilir. Dosya bulunmazsa kart placeholder metnine düşer.

## Dosya Adı Eşleşmesi (10 görsel, 7 araç)

Aşağıdaki dosya adlarını **birebir** kullanın (küçük harf, tire ile ayrılmış, Türkçe karakter yok):

| Sıra | Dosya adı | Galeri kartı | Tema |
|---|---|---|---|
| 1 | `ferrari-purosangue.jpg` | Ferrari Purosangue (¾ ön) | Gümüş — tabela altı |
| 2 | `bmw-m2-competition.jpg` | BMW M2 Competition | Mavi — atölye içi |
| 3 | `mercedes-amg-gtr.jpg` | Mercedes-AMG GT R (¾) | Yeşil — tabela altı, ¾ ön açı |
| 4 | `porsche-911-turbo.jpg` | Porsche 911 Turbo (ön) | Siyah — atölye içi, ¾ ön (Window Film raflar) |
| 5 | `tesla-model-y.jpg` | Tesla Model Y | Gümüş — tabela altı, yeni nesil |
| 6 | `chevrolet-corvette.jpg` | Chevrolet Corvette | Kırmızı — yan profil |
| 7 | `porsche-911-turbo-arka.jpg` | Porsche 911 Turbo (arka) | Siyah — atölye içi, büyük spoiler |
| 8 | `mercedes-amg-gtr-on.jpg` | Mercedes-AMG GT R (önden) | Yeşil — tam ön, gün batımı |
| 9 | `chevrolet-silverado.jpg` | Chevrolet Silverado | Siyah — tabela altı, ¾ ön |
| 10 | `ferrari-purosangue-yan.jpg` | Ferrari Purosangue (yan) | Gümüş — yan profil |

## Boyut & Format

- **Boyut:** 1200×900 px (4:3) — tüm cihazlarda net görünür
- **Format:** JPEG (Progressive önerilir)
- **Hedef dosya boyutu:** 200–400 KB (kalite ~80)
- **Renk profili:** sRGB

## Telefondan Hızlı Yöntem

1. WhatsApp / Galeri'den fotoğrafı seç → **Paylaş** → **Dosyalara Kaydet** (iPhone) / **İndir** (Android)
2. Mac'e AirDrop / e-posta / iCloud Drive ile gönder
3. Mac'te dosyayı yeniden adlandır (tabloda yazan isim)
4. `LlumarMaslak/img/gallery/` klasörüne sürükle-bırak
5. Site otomatik gösterir; ek bir şey yapmana gerek yok

## Yeni Araç Eklemek İçin

1. Görseli bu klasöre yukarıdaki format ile koy (`marka-model.jpg`)
2. `index.html` içinde galeri bölümüne yeni kart ekle:

```html
<div class="gallery-card">
  <div class="gallery-img">
    <img src="img/gallery/marka-model.jpg" alt="Marka Model — LLumar Maslak çalışması" loading="lazy" onerror="this.style.display='none'" />
    <span class="placeholder">Görsel · Marka Model</span>
  </div>
  <div class="gallery-info">
    <div class="car">Marka Model</div>
    <div class="service">Uygulanan Hizmet</div>
  </div>
</div>
```

## Optimizasyon İpuçları

- macOS: Preview → Tools → Adjust Size → 1200 px wide → File → Export → JPEG, Quality 80
- Online: [squoosh.app](https://squoosh.app/) (Google'ın ücretsiz aracı, MozJPEG önerilir)
- Toplu: ImageOptim macOS uygulaması
