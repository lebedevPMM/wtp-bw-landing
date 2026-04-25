# WTP × Bluewaters — landing page

Info-страница для warmup-кампании WTP2 к встрече Bluewaters 6 мая 2026.

**Live:** https://lebedevpmm.github.io/wtp-bw-landing/

## Что внутри

- `index.html` — single-page landing (mobile-first, vanilla CSS+JS)
- 4 блока: Hero / Чем помогаем / 6 мая на встрече BW / Опц. форма (accordeon)
- Primary CTA: `https://t.me/Olga_WTP` (placeholder — заменить на финальный handle)
- UTM capture в sessionStorage
- Form submit → открывает Telegram с prefilled-сообщением

## TODO до прод-запуска

- [ ] Заменить `Olga_WTP` на финальный TG-handle Оли (5 мест: hero CTA, event CTA, footer, form JS, success block)
- [ ] Подключить GA4 (вставить gtag перед `</head>` если хотим трекать клики/submit)
- [ ] Добавить OG-image `og-image.png` (1200×630, navy + gold + portrait Оли)
- [ ] Перенести на `wtp.ae/bw` когда нужно

## Локально

```bash
cd ~/Desktop/wtp-bw-landing
python3 -m http.server 8000
open http://localhost:8000
```

## Deploy

GitHub Pages, branch `main`, root `/`.
