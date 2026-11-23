# Nova Raiders

Tarayıcıda çalışan 3D nişancı oyunu prototipi. Oyun, depodaki ZIP paketlerinden glTF/GLB karakter ve silah modellerini çalışma anında açar; modeller yüklenemezse basit yedek görselleri gösterir.

## Çalıştırma

ZIP dosyaları ve sayfa aynı dizinde bulunmalı. `file://` yerine yerel web sunucusu kullanın:

```bash
python3 -m http.server 8080
```

Ardından `http://localhost:8080` adresini açın. Three.js ve JSZip CDN'den yüklendiği için internet bağlantısı gerekir. GitHub Pages'te çalıştırmak için `fortnite-clone-game` dalını yayınlayın.

## Kontroller

- **WASD** — Hareket
- **Fare** — Bakış / nişan
- **Sol tık** — Ateş
- **Boşluk** — Zıpla
- **Shift** — Koş
- **R** — Şarjör doldur

## Kullanılan paketler

- `KayKit_Character_Animations_1.1.zip` — karakter modelleri
- `kenney_blaster-kit_2.1.zip` — blaster modelleri
- `kenney_prototype-kit.zip` — depoda mevcut; dekor/arayüz prototip paketi

Oyun, karakter ve silah paketlerindeki ilk uygun glTF/GLB modelini bulup yüklemeyi dener. Paket lisanslarına ve atıf koşullarına ZIP'lerin içindeki dosyalardan bakın.
