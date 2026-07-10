# Kyrzma Studios — Yasal Belgeler

Bu repo, **Kyrzma Studios** tarafından yayınlanan tüm mobil oyunların yasal
belgelerini (Gizlilik Politikası ve Kullanım Koşulları) barındıran tek merkezi
sitedir. GitHub Pages ile statik olarak yayınlanır; harici bağımlılık yoktur,
tüm sayfalar kendi içinde (self-contained) ve mobil uyumludur.

## Yapı

```
/
├── index.html                 Stüdyo açılış sayfası (oyunlar + belge linkleri, EN/TR)
├── privacy/
│   └── index.html             Stüdyo geneli Gizlilik Politikası (EN/TR)
├── terms/
│   └── index.html             Stüdyo geneli Kullanım Koşulları (EN/TR)
├── lanternfall/
│   ├── privacy.html           LANTERNFALL'un orijinal gizlilik metni (arşiv, birebir)
│   └── terms.html             LANTERNFALL'un orijinal koşullar metni (arşiv, birebir)
├── lanternfall-privacy.html   Yönlendirme → privacy/ (geriye uyumluluk)
├── terms.html                 Yönlendirme → terms/ (geriye uyumluluk)
└── README.md
```

- **Canlı belgeler** `privacy/` ve `terms/` altındadır ve tüm oyunları kapsar.
- **`lanternfall/`** klasörü, LANTERNFALL'un ilk yayınında kullanılan orijinal
  tekil metinleri arşiv olarak korur (geçmiş referans için değiştirilmez).
- Kök dizindeki `lanternfall-privacy.html` ve `terms.html` eski bağlantıların
  kırılmaması için meta-refresh ile yeni adreslere yönlendiren küçük sayfalardır.

## GitHub Pages

Site, deponun GitHub Pages ayarından (Settings → Pages, `main` dalı / kök) yayınlanır.
Yayın adresi depo adına bağlıdır: `https://<kullanıcı>.github.io/<repo-adı>/`.

> Not: Depo adı değiştirilirse (ör. `kyrzma-studios`) Pages adresi de değişir ve
> **eski adres yönlenmez**. Mağaza (Play Console / App Store Connect) gizlilik
> URL'lerini yeni adrese göre güncellemeyi unutmayın.

## Yeni oyun eklerken

1. `privacy/index.html` içindeki **"Scope of This Policy" / "Bu Politikanın Kapsamı"**
   bölümüne yeni oyunun adını ve paket adını (ör. `com.kyrzma.<oyun>`) ekleyin
   (hem EN hem TR bloklarına).
2. Gerekiyorsa `terms/index.html` giriş paragrafındaki örnek oyun listesine
   yeni oyunu ekleyin (hem EN hem TR).
3. `index.html` (açılış sayfası) içindeki **Games / Oyunlar** listesine oyunu ve
   durumunu (Live / In development) ekleyin.
4. Sayfaların altındaki "Last updated / Son güncelleme" tarihini güncelleyin.

## İletişim

ykbgonder@gmail.com
