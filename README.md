# Meteor Avcısı — 2D Uzay Oyunu

Yapımcı: **Ekrem Malik**

React + Vite + HTML5 Canvas. Harici oyun motoru yok.

## Oyna

https://ekrem-malik.github.io/meteor-avcisi/

`main` dalına yapılan her değişiklik otomatik olarak yayınlanır.

## Çalıştırma

```bash
npm install
npm run dev      # http://localhost:5173
npm run build    # dist/ klasörüne üretim çıktısı
```

## Kontroller

| Tuş | İşlev |
| --- | --- |
| ← → | Hareket |
| SPACE | Ateş |
| P | Duraklat / devam |

## Yapı

```
src/
  game/          # React'ten bağımsız oyun mantığı
    config.js    # Tüm denge ayarları (hız, puan, zorluk)
    entities.js  # Gemi, mermi, meteor, parçacık, yıldız üretimi
    engine.js    # Güncelleme döngüsü, çarpışma, zorluk
    render.js    # Canvas çizimi
    input.js     # Klavye → soyut girdi (mobil kontroller buraya bağlanacak)
    storage.js   # En yüksek skor (localStorage)
  components/    # GameCanvas, HUD, PauseOverlay, GameOverScreen
  App.jsx        # Ekran durumları ve yeniden başlatma
```
