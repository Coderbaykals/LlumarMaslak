# Galeri Görselleri

Bu klasöre yüklenen JPG dosyaları, `index.html` içindeki galeri kartlarında otomatik gösterilir. Dosya bulunmazsa kart placeholder metnine düşer.

## Dosya Adı Eşleşmesi (5 araç, 5 dosya)

Aşağıdaki dosya adlarını **birebir** kullanın (küçük harf, tire ile ayrılmış, Türkçe karakter yok):

| Dosya adı | Galeri kartı | Açıklama |
|---|---|---|
| `ferrari-purosangue.jpg` | Ferrari Purosangue | Gümüş, ¾ ön açı, tabela altında |
| `bmw-m2-competition.jpg` | BMW M2 Competition | Mavi, atölye içi, ¾ ön |
| `porsche-911-turbo.jpg` | Porsche 911 Turbo | Siyah, atölye içi, arka |
| `chevrolet-silverado.jpg` | Chevrolet Silverado | Siyah, tabela altı, ¾ ön |
| `ferrari-purosangue-yan.jpg` | Ferrari Purosangue (yan) | Gümüş, yan profil, tabela altı |

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
