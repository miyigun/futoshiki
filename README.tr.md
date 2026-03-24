# futoshiki

Cyberpunk temalı, tarayıcı tabanlı bir Futoshiki bulmaca oyunu. Neon görsel efektler, animasyonlu arka plan ve tam responsive destekle tek sayfalık bir HTML uygulaması olarak geliştirilmiştir.

---

## Özellikler

### 1. Oyun Tahtası
- **4×4 ve 5×5** ızgara modları
- Eşitsizlik sembolleri: `<` / `>` (yatay), `∧` / `∨` (dikey) — sembolün ucu her zaman küçük değeri gösterir

### 2. Zorluk Seviyeleri
- **KOLAY / ORTA / ZOR** — verilen hücre sayısı ve geri sayım süresi değişir
  - 4×4: Kolay = 2 dk, Orta = 3 dk, Zor = 4,5 dk
  - 5×5: Kolay = 4 dk, Orta = 6 dk, Zor = 8 dk

### 3. Geri Sayım Zamanlayıcısı
- Zorluk seviyesine göre belirlenen süreden geri sayar
- Son 10 saniyede kırmızıya döner ve pulse animasyonu oynar

### 4. Kontroller
- **Numpad:** rakam tuşları (1–N) + ✕ (silme) butonu
- **SIFIRLA** — mevcut bulmacayı yeniden başlatır
- **ÇÖZÜM** — tüm çözümü gösterir
- **KONTROL ET** — mevcut ilerlemeyi doğrular

### 5. Başarı Modalı
- Bulmaca doğru çözüldüğünde **"ERİŞİM ONAYLANDI"** ekranı gösterilir

### 6. Arka Plan Müziği
- Yüklendiğinde `mp3/music.mp3` otomatik başlar
- ♪ / × butonu ile açılıp kapatılabilir

### 7. Yardım Butonu (?)
- Oyunu sıfırlamadan kural modalını açar

### 8. Cyberpunk Görsel Tema
- Scanlines, neon grid pulse, yüzen parçacık animasyonları
- Glassmorphism paneller, Orbitron & Rajdhani Google Fontları

### 9. Responsive Tasarım
- Mobil (dikey), tablet ve masaüstü için optimize edilmiştir
- Mobilde yatay modda döndürme uyarısı gösterilir

### 10. Bulmaca Çözücü
- `minimizeInequalities` fonksiyonu, üretilen her bulmacada tek geçerli çözümü garanti eder

---

## Proje Yapısı

```
futoshiki/
├── index.html    — tam uygulama (HTML/CSS/JS tek dosya)
└── mp3/
    └── music.mp3 — arka plan müziği
```

---

## Başlangıç

1. Repoyu klonlayın:
   ```bash
   git clone https://github.com/miyigun/futoshiki.git
   ```
2. Proje klasörüne girin:
   ```bash
   cd futoshiki
   ```
3. `index.html` dosyasını tarayıcınızda açın — derleme veya sunucu gerekmez.

---

## Nasıl Oynanır

1. Izgara boyutu (**4×4** veya **5×5**) ve zorluk seviyesi (**KOLAY**, **ORTA** veya **ZOR**) seçin.
2. Her hücreyi, her satır ve sütunda her rakam tam olarak bir kez geçecek şekilde doldurun.
3. Tüm eşitsizlik işaretlerine uyun — `<`, `>`, `∧`, `∨` sembollerinin ucu her zaman küçük sayıya doğru bakar.
4. İlerlemenizi doğrulamak için **KONTROL ET** butonunu kullanın.
5. Takıldınız mı? **ÇÖZÜM** butonu ile doğru cevabı görün ya da **SIFIRLA** ile baştan başlayın.
6. Geri sayım sona ermeden bulmacayı çözün!

---

## 🛠️ Kullanılan Teknolojiler

- HTML5 / CSS3 / Vanilla JavaScript
- [Tailwind CSS](https://tailwindcss.com/) (CDN üzerinden)
- [jQuery](https://jquery.com/) 3.7.1
- [Google Fonts](https://fonts.google.com/) — Orbitron & Rajdhani

---

## 📌 Notlar

- Kurulum veya derleme aracına gerek yoktur — yalnızca `index.html` dosyasını açın.
- Bulmaca üreteci her seferinde tek ve geçerli çözüme sahip bir tahta oluşturur.
- Arka plan müziği tarayıcının otomatik oynatma iznini gerektirir; başlamazsa ♪ / × butonu ile etkinleştirin.
- Oyun tamamen tek bir `index.html` dosyasında yer almaktadır.

---

## 📜 Lisans

Bu proje MIT lisansı altında sunulmaktadır. Ayrıntılar için LICENSE dosyasına bakınız.