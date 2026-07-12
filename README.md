# Kyrzma Studios

Bu repo, **Kyrzma Studios**'un resmî web sitesi ile yasal belgelerinin
(Gizlilik Politikası ve Kullanım Koşulları) tek kaynağıdır. GitHub Pages ile
statik olarak yayınlanır; harici bağımlılık yoktur, tüm sayfalar kendi içinde
(self-contained) ve mobil uyumludur.

## Yapı

```
/
├── index.html          Stüdyo sayfası (banner hero + hakkımızda + kurucu + oyun vitrini + blog listesi + belge linkleri, TR/EN — varsayılan TR)
├── blog/
│   └── <yazı>/index.html   Blog yazıları (TR asıl + EN çeviri, tema aynı)
├── privacy/
│   └── index.html      Stüdyo geneli Gizlilik Politikası (EN/TR)
├── terms/
│   └── index.html      Stüdyo geneli Kullanım Koşulları (EN/TR)
├── assets/             Marka görselleri (banner, logo, favicon)
│   └── games/          Oyun ikonları (roadloom, perisar, lanternfall)
├── sitemap.xml         Site haritası (mutlak URL'ler)
├── robots.txt          Sitemap işaretçisi
├── .gitignore
└── README.md
```

Tasarım tek koyu tema (siyah zemin + metalik gümüş vurgu), marka görselleriyle
uyumludur; tüm görseller repo içindedir, harici bağımlılık yoktur.

## GitHub Pages

Site, deponun GitHub Pages ayarından (Settings → Pages, `main` dalı / kök)
yayınlanır. Yayın adresi depo adına bağlıdır:
`https://<kullanıcı>.github.io/<repo-adı>/`.

> Not: Depo adı değişirse Pages adresi de değişir ve eski adres yönlenmez.
> Mağaza (Play Console / App Store Connect) gizlilik URL'lerini yeni adrese göre
> güncellemeyi unutmayın.

## Yeni oyun eklerken

**Yasal belgeler için hiçbir güncelleme gerekmez.** Gizlilik Politikası ve
Kullanım Koşulları stüdyo geneli yazılmıştır; belirli oyun adı veya paket adı
içermez, bu yüzden Kyrzma Studios adı altında yayınlanan her oyunu otomatik
olarak kapsar. Aynı belgeleri ve aynı URL'leri tüm oyunlarınız için
kullanabilirsiniz.

Ana sayfadaki **Oyunlar / Games** vitrinine oyun eklemek için: ikonu
`assets/games/` içine koyun ve `index.html` içindeki `.games` bloğuna mevcut
kartları örnek alarak yeni bir `<a class="game" …>` kartı ekleyin (Play Store
linki + `data-en`/`data-tr` açıklamalar). Metinlerde yalnızca gerçek oynanışı
anlatın; pazarlama abartısı kullanmayın.

Yalnızca içerik değişirse sayfaların üstündeki "Son güncelleme / Last updated"
tarihini yenileyin.

## İletişim

ykbgonder@gmail.com
