# LLumar Maslak

Maslak, İstanbul'da yetkili LLumar uygulama atölyesinin resmi web sitesi.

**Canlı:** https://coderbaykals.github.io/LlumarMaslak/

## Hizmetler

- Otomobil Cam Filmi — LLumar (ATC, ATR, CTXI, AIR 80, IRX)
- Boya Koruma Filmi (PPF) — LLumar Platinum, Valor & STEK
- Cam Çatlağı Tamiri

## İletişim

- Sabit: +90 212 276 93 56
- WhatsApp / Mobil: +90 507 333 07 03
- Pzt – Cum 09:00 – 19:00 · Cmt 09:00 – 17:00
- Maslak Mahallesi, Sarıyer / İstanbul

## Stack

Tek dosya, vanilla HTML / CSS / JS. Build adımı yok. GitHub Pages üzerinden yayınlanır.

## Dosya Yapısı

```
index.html              Ana sayfa
kvkk.html               KVKK Aydınlatma Metni
gizlilik.html           Gizlilik Politikası
cerez-politikasi.html   Çerez Politikası
404.html                Bulunamadı sayfası
manifest.webmanifest    PWA manifest
robots.txt              Crawler yol haritası (AI crawler'lar açık)
sitemap.xml             Site haritası (tüm sayfalar)
llms.txt                AI motorları için yapılandırılmış özet
og-image.jpg            Sosyal paylaşım görseli (EKLENECEK)
README.md               Bu dosya
```

## SEO / AEO

- Schema.org JSON-LD: AutomotiveBusiness, FAQPage, BreadcrumbList, WebSite
- Open Graph + Twitter Card
- Geo metadata (Maslak/İstanbul, 41.1086, 29.0186)
- robots.txt AI crawler'lara açık (GPTBot, PerplexityBot, ClaudeBot, Google-Extended, vb.)
- llms.txt AI motorları için

## Production Fonksiyonları

- **Form gönderim:** Formspree integration. `index.html` içinde `action="https://formspree.io/f/YOUR_FORMSPREE_ID"` — yayın öncesi gerçek ID ile değiştirilecek.
- **Honeypot:** Hidden `_gotcha` field, spam botlarını sessizce filtreler.
- **KVKK rıza:** Form'da zorunlu açık rıza checkbox.
- **Cookie banner:** İlk ziyarette KVKK uyumlu banner, localStorage'da tercih kaydı.
- **Analytics:** Google Analytics 4 (consent sonrası yüklenir). `index.html` içinde `GA_ID = 'G-XXXXXXXXXX'` — yayın öncesi gerçek Measurement ID ile değiştirilecek.
- **PWA:** Manifest dosyası, "Ana ekrana ekle" desteği.
- **404:** Özel hata sayfası.

## Yayın Öncesi Checklist

- [ ] Formspree hesabı aç ([formspree.io](https://formspree.io)), form ID al
- [ ] `index.html` içinde `YOUR_FORMSPREE_ID` yerine gerçek ID
- [ ] Google Analytics 4 mülkü oluştur, Measurement ID al
- [ ] `index.html` içinde `G-XXXXXXXXXX` yerine gerçek ID
- [ ] `og-image.jpg` ekle (1200×630 px, repo köküne)
- [ ] Custom domain ekle ve `CNAME` dosyası oluştur
- [ ] Schema/canonical/sitemap URL'lerini custom domain'e güncelle
- [ ] Google Search Console + Bing Webmaster Tools'a sitemap submit
- [ ] Google Business Profile kaydı
- [ ] Gerçek galeri görsellerini ekle
- [ ] Sosyal medya hesapları açıldıysa footer link'lerini güncelle
- [ ] KVKK + Gizlilik + Çerez politikası metinlerini hukuk müşaviri inceler
