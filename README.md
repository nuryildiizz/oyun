# Gece Kuşları

Oyun gecelerinin gizli kulübü. Tek telefondan, elden ele oynanan sekiz parti oyunu.
Her oyunun kendine ait bir teması var; oyun seçildiğinde sitenin rengi, yazı tipi ve havası tamamen değişir.

| Oyun | Tema |
| --- | --- |
| Vampir Köylü | Gotik gece, kan kırmızısı, ay ve sis |
| Doğruluk mu Cesaret mi | Gün batımı turuncusu |
| Tabu | Elektrik mavisi ve sarı, pop |
| Casus | Gizli dosya, terminal yeşili |
| Ben Hiç | 70'ler retro, krem ve kiremit |
| Kim Daha Olası | Şeker pastel |
| Sessiz Sinema | Siyah beyaz film, altın |
| Ben Kimim? | Neon atari salonu |

## Çalıştırma

```bash
npm install
npm run dev
```

Tarayıcıda http://localhost:3000 adresini aç.

## Yapı

- `app/page.tsx`: oyun seçme ekranı
- `app/<oyun>/page.tsx`: her oyun kendi klasöründe
- `lib/games.ts`: ana sayfadaki oyun listesi
- `lib/data.ts`: roller, sorular, görevler, kartlar (yeni içerik eklemek için burayı düzenle)
- `app/globals.css`: temalar, `.shell[data-theme="..."]` altındaki renk değişkenleri
- İkonlar: `lucide-react`
