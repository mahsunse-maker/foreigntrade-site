# foreigntrade-site (proje özeti)

> Son güncelleme: 2026-11-16 (genel yayın: tanıtım sayfası, /uygulama, gizlilik)

https://foreigntrade.app sitesinin yayın deposu (herkese açık). Cloudflare Pages `foreigntrade-site` projesi `public/`
klasörünü yayınlar; **`main`'e push = otomatik yayın**. Derleme adımı yok, düz HTML.

- `public/index.html`: tanıtım sayfası (koyu açılış bandı, logo iner, "Tarayıcıda başla"; masalar ve 17 modül uygulamaya bağlanır). Mevzuat değeri içermez; karar kartındaki rakamlar CN_STEEL_01 senaryosundan.
- `public/site.css`: ortak stil ve yazı tipleri (`public/fonts/`, OFL; Google Fonts isteği yok). `public/gizlilik/`: gizlilik politikası (iletişim adresi kullanıcı onayıyla, 16.11.2026).
- `public/og.png` paylaşım görseli, `apple-touch-icon.png`, `icon-192/512.png`, `robots.txt`, `sitemap.xml`.
- `public/apps/`: "Diğer uygulamalarımız" simgeleri (128 px). Yeni uygulama yayınlanınca buraya ve kardeş sitelere eklenir.
- `public/uygulama/`: web uygulaması (foreigntrade.app/uygulama). Elle düzenlenmez; uygulama deposunda `sh scripts/web-yayin.sh` derleyip buraya kopyalar. Rotalar `_redirects`'te; eski `/onizleme` adresi 301 ile buraya gider.
- `public/logo.svg`: logo (Üç konteyner: ithalatçı, ihracatçı, bankacı + safran rıhtım). Elle düzenlenmez; uygulama deposunda `python3 scripts/logo.py` üretir.
- Alan adı foreigntrade.app, ad sunucuları Cloudflare'de. İleride ek alan adları 301 ile buraya bağlanır.
- Sitede resmî kurumlarla bağ olmadığı yazılı kalmalı.

Uygulama deposu: `mahsunse-maker/foreigntrade` (özel, `~/Projeler/foreigntrade`). Uyarı: Pages projesini asla o özel depoya bağlama.

Proje listesi: `~/.claude/CLAUDE.md`.
