# foreigntrade-site (proje özeti)

> Son güncelleme: 2026-11-16 (önizleme eklendi)

https://foreigntrade.app sitesinin yayın deposu (herkese açık). Cloudflare Pages `foreigntrade-site` projesi `public/`
klasörünü yayınlar; **`main`'e push = otomatik yayın**. Derleme adımı yok, düz HTML.

- `public/index.html`: "Yakında" tanıtım sayfası. Rakam ve mevzuat değeri içermez; uygulama hazır olunca değişir.
- `public/apps/`: "Diğer uygulamalarımız" simgeleri (128 px). Yeni uygulama yayınlanınca buraya ve kardeş sitelere eklenir.
- `public/onizleme/`: uygulamanın web önizlemesi (foreigntrade.app/onizleme, arama motorlarına kapalı). Elle düzenlenmez; uygulama deposunda `sh scripts/onizleme.sh` derleyip buraya kopyalar. Rotalar `_redirects`'te, noindex `_headers`'ta.
- `public/logo.svg`: geçici logo ve favicon (espresso zemin, safran ve beyaz karşılıklı oklar).
- Alan adı foreigntrade.app, ad sunucuları Cloudflare'de. İleride ek alan adları 301 ile buraya bağlanır.
- Sitede resmî kurumlarla bağ olmadığı yazılı kalmalı.

Uygulama deposu: `mahsunse-maker/foreigntrade` (özel, `~/Desktop/foreigntrade`). Uyarı: Pages projesini asla o özel depoya bağlama.

Proje listesi: `~/.claude/CLAUDE.md`.
