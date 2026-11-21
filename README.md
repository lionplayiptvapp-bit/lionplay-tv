# LionPlay TV

[![Universal APK](https://img.shields.io/badge/APK-Universal%20(Fire%20TV%20%2B%20Android%20TV)-34C759?style=for-the-badge&logo=android)](https://androidtvfireos.lionplay.workers.dev/apk)
[![Downloader Code](https://img.shields.io/badge/Downloader%20Code-1804273-FF9F0A?style=for-the-badge&logo=amazonfiretv)](https://androidtvfireos.lionplay.workers.dev)
[![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-0A84FF?style=for-the-badge)](LICENSE)

A high-performance, modern dark-glass IPTV player designed specifically for **Amazon Fire TV, Google TV, and Android TV**, built with Kotlin, Jetpack Compose, and hardware-accelerated Media3 / FFmpeg decoding. Fully optimized for television remote controls (D-Pad).

![LionPlay home screen](docs/screenshots/homescreen.jpg)

> **Legal Disclaimer:** LionPlay does not host, provide, or distribute any media content, streams, or playlists. It is an independent player application for personal, legally authorized IPTV sources (Xtream Codes, M3U playlists, Stalker portals).

---

## 📺 Platform & Version Compatibility (Desteklenen Platformlar ve Sürümler)

> **💡 Tek Evrensel APK (Universal APK):**
> Android TV ve Amazon Fire TV için uygulamayı **iki ayrı pakete ayırmaya gerek yoktur.** LionPlay, her iki platformun da sistem kütüphanelerini, D-Pad gezinme motorlarını ve mağaza API'lerini tek bir universal APK içerisinde barındırır. Tek dosya tüm cihazlarda doğrudan en yüksek performansla çalışır.

| Platform | Desteklenen Sürümler (OS Versions) | Uyumlu Popüler Cihazlar (Devices) | Durum |
|---|---|---|---|
| **Amazon Fire TV** | **Fire OS 6, 7, 8**<br>(Android 7.1 Nougat ila Android 11+) | Fire TV Stick (Gen 3, Lite), Fire TV Stick 4K, Fire TV Stick 4K Max, Fire TV Cube, Fire TV Edition Akıllı TV'ler | Tam Uyumlu (%100 Destek) |
| **Google TV** | **Android 10, 11, 12, 13, 14+** | Chromecast with Google TV (HD & 4K), Sony Bravia Google TV, TCL Google TV, Philips Google TV | Tam Uyumlu (%100 Destek) |
| **Android TV** | **Android 6.0 Marshmallow (API 23) ila Android 14+** | Xiaomi Mi Box S, Mi TV Stick 4K, Nvidia Shield TV / Pro, Next, Nokia Streaming Box, tüm Android TV Box'lar | Tam Uyumlu (%100 Destek) |

---

## 🚀 Hızlı Kurulum Rehberi (Quick Installation)

### Yöntem 1: Downloader Uygulaması ile (En Kolay Yöntem)
Televizyonunuzun uygulama mağazasından (Amazon Appstore veya Google Play Store) ücretsiz **Downloader by AFTVnews** uygulamasını açın:

1. Downloader arama çubuğuna **`1804273`** kodunu girin ve **Go** butonuna basın.
2. İndirme otomatik olarak başlayacaktır.
3. İndirme bittiğinde ekrana gelen **Install (Yükle)** butonuna basarak kurulumu tamamlayın.

### Yöntem 2: Doğrudan Web İndirme Bağlantısı
* **Evrensel APK (Universal):** [https://androidtvfireos.lionplay.workers.dev/apk](https://androidtvfireos.lionplay.workers.dev/apk)
* **Web Dağıtım Portalı:** [https://androidtvfireos.lionplay.workers.dev](https://androidtvfireos.lionplay.workers.dev)

### Yöntem 3: ADB / USB Bellek ile Sideload
```bash
adb install -r LionPlay-AndroidTV-FireTV.apk
```

---

## 📱 Çoklu Cihaz Yönetimi & QR Kod Portalı (1 Lisans = 5 Cihaz)

LionPlay tek bir lisans ile **5 farklı televizyona kadar** eşzamanlı kullanımı destekler:
* **Kumandasız Aktivasyon:** TV ekranında beliren dinamik QR kodu telefon kameranızla okutarak, kumandayla harf yazmak zorunda kalmadan lisansınızı telefonunuzdan anında tanımlayabilirsiniz.
* **Cihazları Yönetme & Silme:** Telefondan açılan yönetim portalında (`/devices?code=...`) lisansınıza bağlı 5 cihaza kadar tüm televizyon modellerini görebilir, eski veya kullanmadığınız cihazları tek dokunuşla silerek yeni TV'ler için yer açabilirsiniz.
* **⚠️ Güvenlik Uyarısı:** Cihaz yönetim bağlantısı ve QR kod cihazınıza özeldir. Cihazlarınızın yetkisiz silinmesini önlemek için bu linki üçüncü şahıslarla paylaşmayın.

---

## 🔄 Uygulama İçi Güncelleme Sistemi (OTA Updates)

Uygulamanızı güncellemek için yeniden kurulum yapmanıza veya dosya aramanıza gerek yoktur:
* **Otomatik Kontrol (ON / OFF):** **Ayarlar ➔ Hakkında (About)** menüsünden otomatik güncelleme denetimini açıp kapatabilirsiniz. Açık olduğunda her uygulama başlangıcında yeni sürümü sessizce kontrol eder.
* **Şimdi Güncelleme Ara (Manuel):** `Check for updates now` butonuna basarak en son sürümü anında sorgulayabilirsiniz. Yeni sürüm çıktığında tek tıkla doğrudan TV üzerinden indirip kurabilirsiniz.
* **Veri Güvencesi:** Güncellemeler sırasında oynatma listeleriniz (M3U / Xtream), favorileriniz, izleme geçmişiniz ve lisans ayarlarınız **kesinlikle silinmez, eksiksiz korunur**.

---

## 🌟 Öne Çıkan Özellikler (Core Features)

* **Oynatma Listeleri:** Xtream Codes, M3U URL / dosya ve Stalker portal desteği. Çoklu liste birleştirme ("Also show").
* **Multi-View:** Aynı anda 4 farklı canlı yayını tek ekranda donmadan izleme imkanı.
* **Gerçek Zamanlı AI Altyazı:** Yabancı canlı yayınlarda ve filmlerde anlık Türkçe altyazı ve ses çevirisi.
* **Gelişmiş Oynatıcı:** Media3 (ExoPlayer) + FFmpeg AC3/E-AC3/DTS ses çözücü, 4K HDR desteği, otomatik kare hızı eşleme (AFR / Auto-FPS).
* **EPG & Catchup:** Geriye dönük yayın arşivi ve program hatırlatıcıları.
* **Apple tvOS Tasarım Dili:** Akıcı animasyonlar, 12 renk teması ve koyu cam (dark glass) estetiği.

---

## 📸 Ekran Görüntüleri (LionPlay TV Screenshots)

| 🏠 Ana Sayfa (Home Screen) | ⚙️ Ayarlar (Settings & Hub) |
|---|---|
| ![LionPlay Home](docs/screenshots/homescreen.jpg)<br>**Ana Sayfa** – 👑 LIONPLAY üst gezinme menüsü, son izlenen canlı yayınlar ve en yeni filmler | ![LionPlay Settings](docs/screenshots/settings.jpg)<br>**Ayarlar** – Apple tvOS koyu cam tasarım, hesap yönetimi ve cihaz QR portalı |

---

## ❓ Sıkça Sorulan Sorular (FAQ)

<details>
<summary><b>1. Fire TV için ayrı, Google TV için ayrı APK indirmem gerekir mi?</b></summary>
Hayır. LionPlay evrensel (Universal) mimariyle derlenmiştir. Tek bir APK dosyası tüm Android TV, Google TV ve Amazon Fire TV cihazlarında eksiksiz çalışır.
</details>

<details>
<summary><b>2. Güncelleme yaparsam kayıtlı kanallarım veya ayarlarım gider mi?</b></summary>
Hayır. LionPlay'in tüm güncellemeleri mevcut veritabanını, lisansınızı ve listelerinizi koruyarak sistem üzerine yama olarak kurulur.
</details>

<details>
<summary><b>3. Bir lisans kodunu kaç farklı cihazda kullanabilirim?</b></summary>
LionPlay Premium lisansı ile 5 farklı televizyon cihazını aktif edebilirsiniz. Cihaz limitiniz dolduğunda TV'nizdeki QR kodu telefonunuzla okutarak eski cihazları tek tıkla silebilirsiniz.
</details>

<details>
<summary><b>4. Uygulama içi API anahtarları (TMDB / OMDb) zorunlu mudur?</b></summary>
Zorunlu değildir. Sağlayıcınızın kendi afiş ve bilgileri doğrudan kullanılır. Ancak TMDB ve OMDb ücretsiz anahtarlarını girerseniz filmlerin Türkçe açıklamaları, IMDb puanları ve oyuncu kadrosu otomatik zenginleştirilir.
</details>

---

## 🛠️ Kaynak Koddan Derleme (Building)

Gereksinimler: Android Studio (Ladybug veya üstü), JDK 17, Android SDK.

```bash
git clone https://github.com/lionplayiptvapp-bit/android.git
cd android
./gradlew assembleRelease
```
Derlenen APK dosyası `app/build.nosync/outputs/apk/release/app-release.apk` dizininde üretilir.

---

## 📄 Lisans & Telif Hakkı

Copyright (C) 2026 LionPlay TV Contributors.  
LionPlay, **GNU General Public License v3.0 (GPL-3.0)** kapsamında yayınlanan özgür ve açık kaynak kodlu bir yazılımdır. FFmpeg native audio decoder kütüphanesi içermektedir. Detaylar için [LICENSE](LICENSE) dosyasına göz atabilirsiniz.
