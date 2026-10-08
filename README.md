# Hisar Tekin İnşaat — Kurumsal Portfolyo

Statik, bağımlılıksız site. `index.html` doğrudan herhangi bir hostingde (Netlify, Vercel, GitHub Pages, cPanel) çalışır.

- `hero.mp4` — kaydırmaya bağlı oynayan hero videosu (sık keyframe ile kodlandı, `-g 8`). Yeni video ile değiştirmek için aynı adla üzerine yazın ve
  `ffmpeg -i yeni.mp4 -an -vf scale=1280:-2 -c:v libx264 -crf 26 -g 8 -movflags +faststart hero.mp4` ile kodlayın.
- `img/` — web için optimize edilmiş proje fotoğrafları (webp).
- `assets/img/` — orijinal fotoğraflar (AI video üretiminde başlangıç karesi olarak kullanılıyor).
- Diller: `index.html` içindeki `EN` sözlüğü. Yeni dil eklemek için aynı anahtarlarla yeni bir nesne ekleyip `DICT`'e ve dil butonlarına ekleyin.
