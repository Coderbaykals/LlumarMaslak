# Galeri Görselleri

Bu klasöre yüklenen JPG dosyaları, `index.html` içindeki galeri kartlarında otomatik gösterilir. Dosya bulunmazsa kart placeholder metnine düşer.

## Dosya Adı Eşleşmesi

Aşağıdaki dosya adlarını **birebir** kullanın (Türkçe karakter yok, küçük harf, tire ile ayrılmış):

| Dosya adı | Galeri kartı |
|---|---|
| `ferrari-purosangue.jpg` | Ferrari Purosangue |
| `bmw-m2-competition.jpg` | BMW M2 Competition |
| `mercedes-amg-gtr.jpg` | Mercedes-AMG GT R (yeşil) |
| `chevrolet-corvette.jpg` | Chevrolet Corvette (kırmızı) |
| `chevrolet-silverado.jpg` | Chevrolet Silverado (siyah) |
| `tesla-model-y.jpg` | Tesla Model Y (mat gri) |

## Boyut & Format

- **Boyut:** 1200×900 px (4:3) — tüm cihazlarda net görünür
- **Format:** JPEG (Progressive önerilir)
- **Hedef dosya boyutu:** 200–400 KB (kalite ~80)
- **Renk profili:** sRGB

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
