# High-Reliability Analog Front-End (AFE) Design

Bu proje, savunma sanayii standartları göz önünde bulundurularak, gürültülü (EMI) ortamlarda sensör verilerini güvenle işlemek için geliştirilmiş bir **Analog Ön-Uç (AFE)** devresidir. Yıldız Teknik Üniversitesi Biyomedikal Mühendisliği 2. sınıf öğrencisi olarak, teorik devre analizlerini profesyonel tasarım araçlarıyla pratiğe dökmeyi amaçladım.

## 🚀 Proje Özellikleri
* **Giriş Koruma Katmanı:** +/- 15.7V clamping yapısı ile op-amp ve hassas bileşenler aşırı gerilime karşı korunmuştur.
* **Enstrümantasyon Amplifikatörü (InA):** 3-Op-Amp mimarisi ile yüksek CMRR (Ortak Mod Bastırma Oranı) sağlanmıştır.
* **Aktif Filtreleme:** 1 kHz kesim frekanslı 2. derece Sallen-Key Alçak Geçiren Filtre ile yüksek frekanslı parazitler süzülmüştür.
* **Üretim Analizi:** Monte Carlo analizi (100 run) ile komponent toleranslarının seri üretimdeki etkileri simüle edilmiştir.

## 🛠 Kullanılan Teknolojiler
* **Simülasyon:** OrCAD PSpice Designer (Transient, AC Sweep, Noise, Monte Carlo)
* **PCB Tasarımı:** KiCad (2-Layer, Ground Plane, Decoupling Optimization)

## 📁 Klasör Yapısı
* `/Donanim`: KiCad şematik (.kicad_sch) ve PCB (.kicad_pcb) dosyaları.
* `/Simulasyon`: PSpice analiz çıktıları ve grafikler.
* `/Raporlar`: Detaylı proje raporu (PDF) ve 3D tasarım görselleri.

## ⚠️ Gelişim Notları
Bu proje benim için bir öğrenme sürecidir. Şu anki tasarımda genel amaçlı `uA741` op-amp kullanılmıştır. Projenin bir sonraki aşamasında, daha düşük gürültü (Low-noise) değerlerine sahip `OP07` veya `LT1028` gibi modellerle revize edilmesi planlanmaktadır.

---
**Hazırlayan:** Göktan Sarıkan (Yıldız Teknik Üniversitesi)
