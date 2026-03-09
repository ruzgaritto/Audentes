# 🚀 Audentes — Proje Takvimi & Toplantı Ajandası
**Toplantı Tarihi:** 9 Mart 2026  
**Kalan Süreler:** PSR → **16 gün** · PDR → **112 gün** · Final → ~**200 gün**

---

## 🏗️ Takım Şeması

| Kişi | Rol | Teknik Sorumluluklar |
|---|---|---|
| 👑 **Ahmet Taha Çelik** | Kaptan | Proje yönetimi · Mimari kararlar · Model değerlendirme · Rapor koordinasyonu · Klinik eşik optimizasyonu · T3KYS yükleme |
| 👤 **Ali Andaç Erdaş** | Veri Mühendisi | ClinVar/gnomAD veri indirme · EDA · Ön işleme pipeline · Feature engineering · SMOTE/Augmentasyon |
| 👤 **Gizem Öksüz** | Model Geliştirici | Baseline model (LightGBM) · Hiperparametre optimizasyonu · Deney tasarımı · ESM entegrasyon desteği |
| 👤 **Ebrar Yılmaz** | Protein Dil Modelleri | ESM-1v/ESM-2 embedding · Model değerlendirme · Hata analizi |
| 👤 **Songül Sevinti** | Analiz & Görselleştirme | SHAP analizi · Görselleştirme · IEEE referanslar · Veri ön işleme desteği |

### Teknik Sorumluluk Matrisi

| Alan | Ahmet Taha | Ali Andaç | Gizem | Ebrar | Songül |
|---|---|---|---|---|---|
| Proje yönetimi | 🔴 Ana | — | — | — | — |
| Mimari kararlar | 🔴 Ana | 🟡 Destek | 🟡 Destek | 🟡 Destek | — |
| Veri indirme & EDA | 🟡 Destek | 🔴 Ana | — | — | 🟡 Destek |
| Veri ön işleme | 🟡 Destek | 🔴 Ana | — | — | 🟡 Destek |
| Baseline model | 🟡 Destek | — | 🔴 Ana | — | — |
| ESM embedding | 🟡 Destek | — | 🟡 Destek | 🔴 Ana | — |
| SHAP & görselleştirme | 🟡 Destek | — | 🟡 Destek | — | 🔴 Ana |
| Klinik eşik optimizasyonu | 🔴 Ana | — | 🟡 Destek | 🟡 Destek | — |
| Model değerlendirme | 🔴 Ana | — | 🟡 Destek | 🟡 Destek | 🟡 Destek |
| Rapor yazımı | 🔴 Ana | 🟡 Bölüm 3 | 🟡 Bölüm 4 | 🟡 Bölüm 2 | 🟡 Bölüm 6 |
| T3KYS yükleme | 🔴 Ana | — | — | — | — |

---

## 📋 Toplantı Ajandası

### Gündem 1 — Yarışma Özeti 

| Alan | Bilgi |
|---|---|
| **Problem** | Missense genetik varyant → Patojenik mi? Benign mi? |
| **Veri** | ClinVar + gnomAD + ClinGen |
| **Ana Metrik** | Macro F1-score |
| **Değerlendirme** | %90 Algoritma + %10 Sunum |
| **Ödül (1.)** | 180.000 TL |

---

### Gündem 2 — PSR ve Puan Dağılımı 

| # | Bölüm | Puan | Rapor Sorumlusu |
|---|---|---|---|
| 1 | Takım Şeması | — | Ahmet Taha |
| 2 | Literatür Özeti | **10** | Ebrar + Gizem |
| 3 | Veri ve Yöntem | **30** | Ali Andaç + Songül |
| 4 | Deney Tasarımı ve Sonuçlar | **25** | Gizem |
| 5 | Gerekçe, Kaynak ve Özgünlük | **25** | Ahmet Taha |
| 6 | Referanslar (IEEE) | — | Songül |

> **Toplam 90 puan — her puan kritik.**

---

### Gündem 3 — Teknik Mimari 

```
Ham Veri (ClinVar + gnomAD)
        ↓
Veri Filtreleme & Ön İşleme  (Ali Andaç + Songül)
        ↓                    ↓
 Tablo Özellikleri      Protein Dizisi
 gnomAD_AF, CADD,       (ESM-2 embedding)
 SIFT, REVEL, vb.            ↓
        ↓             MLP / Linear Layer
   LightGBM                  ↓
        ↓         ←──────────┘
      Ensemble (Stacking)
              ↓
   Patojenik / Benign Tahmini
              ↓
    SHAP Açıklanabilirlik
```

---

### Gündem 4 — Makale Dağılımı
*(Detay: `makale_dagilimi.md`)*

| Kişi | Okuyacağı Makaleler |
|---|---|
| **Ahmet Taha** | ACMG/AMP 2015 · gnomAD v2 2020 · gnomAD v4 2024 |
| **Ali Andaç** | REVEL 2016 · ClinPred 2018 · BioData Mining 2026 |
| **Gizem** | AlphaMissense 2023 · PreMode 2025 |
| **Ebrar** | ESM-1v 2021 · ESM-2 2023 · DIVA 2025 |
| **Songül** | CADD 2019 · CADD v1.7 2024 · Graph Embed 2025 |

Her kişi kendi makale(leri) için şu 5 soruyu yanıtlayacak:
1. Problem ne? 2. Hangi veri? 3. Hangi yöntem? 4. F1/AUC? 5. Bizim projemizle ilişkisi?

---

### Gündem 5 — Takvim & Görev Dağılımı 
*(Detaylar aşağıdaki tam proje takviminde)*

---
### Gündem 6 — Sonraki Toplantı Tarihi 
Öneri: **14 Mart** — İlk ilerleme check-in'i (veri erişimi + makale özetleri)

---

## 📅 Tam Proje Takvimi

---

### 🔴 FAZA 1 — PSR (Proje Sunuş Raporu)
**9 Mart – 25 Mart 2026** · 16 gün

| Gün | Tarih | Görev | Sorumlu | Çıktı |
|---|---|---|---|---|
| 1 | 9 Mar | Makale okuma başlangıcı | Herkes | — |
| 1–3 | 9–11 Mar | ClinVar + gnomAD veri erişimi, EDA başlangıcı | Ali Andaç + Ahmet Taha | EDA raporu |
| 1–3 | 9–11 Mar | Makale özetleri (5 soru formatı) | Herkes | Özet dokümanı |
| 4–6 | 12–14 Mar | Veri ön işleme pipeline (filtreleme, normalizasyon) | Ali Andaç + Songül | Temiz dataset |
| 4–6 | 12–14 Mar | **Check-in Toplantısı 1** | Tüm ekip | İlerleme raporu |
| 7–9 | 15–17 Mar | Baseline model: LightGBM → F1 skoru al | Gizem | Baseline F1 |
| 10–11 | 18–19 Mar | ESM-2 embedding deneme entegrasyonu | Ebrar | Embedding vektör |
| 12–13 | 20–21 Mar | SHAP analizi + görsel hazırlık | Songül + Gizem | SHAP grafikleri |
| 12–13 | 20–21 Mar | **Check-in Toplantısı 2** | Tüm ekip | Model sonuçları |
| 13–15 | 21–23 Mar | Rapor yazımı (tüm bölümler paralel) | Herkes | Bölüm taslakları |
| 15–16 | 23–24 Mar | Rapor birleştirme + IEEE referanslar | Ahmet Taha + Songül | Tam taslak |
| 16 | 24 Mar | Son gözden geçirme (tüm ekip okur) | Tüm ekip | Onaylı rapor |
| **17** | **25 Mar** | **T3KYS'ye yükleme** | **Ahmet Taha** | **✅ PSR TESLİM** |

---

### 🟡 FAZA 2 — Geliştirme Dönemi
**26 Mart – 28 Haziran 2026** · ~95 gün

| Dönem | Tarih | Görev | Sorumlu |
|---|---|---|---|
| Sprint 1 | 26 Mar – 10 Nis | Model iyileştirme: Ensemble (LightGBM + ESM-2 Stacking) | Gizem + Ebrar |
| Sprint 1 | 26 Mar – 10 Nis | Hiperparametre optimizasyonu (Optuna) | Gizem |
| Sprint 1 | 26 Mar – 10 Nis | Veri augmentasyon denemeleri (SMOTE) | Ali Andaç |
| Sprint 2 | 11 Nis – 25 Nis | Klinik risk odaklı eşik optimizasyonu | Ahmet Taha + Gizem |
| Sprint 2 | 11 Nis – 25 Nis | SHAP + Feature importance kapsamlı analiz | Songül |
| Sprint 2 | 11 Nis – 25 Nis | Hata analizi: Yanlış sınıflanan varyantlar | Ebrar |
| Sprint 3 | 26 Nis – 15 May | AlphaMissense skor entegrasyonu (feature olarak) | Gizem + Ebrar |
| Sprint 3 | 26 Nis – 15 May | Ablation study: Her özelliğin katkısı | Ali Andaç |
| Sprint 4 | 16 May – 15 Haz | Model finalizasyonu + kapsamlı benchmark | Tüm ekip |
| Sprint 4 | 16 May – 15 Haz | PDR yazım hazırlığı | Ahmet Taha |
| Son | 16–28 Haz | PDR yazımı + son gözden geçirme | Tüm ekip |

---

### 🟠 FAZA 3 — PDR (Proje Detay Raporu)
**29 Haziran 2026**

| Tarih | Görev | Sorumlu |
|---|---|---|
| **29 Haziran** | **PDR Teslimi (T3KYS)** | Ahmet Taha |

PDR, PSR'den farklı olarak **tam sonuçları** içerecek:
- Final model mimarisi ve performansı
- Ablation study sonuçları
- Kapsamlı SHAP analizi
- Gerçek klinik uygulama senaryosu

---

### 🟢 FAZA 4 — Finale Hazırlık
**Temmuz – Eylül 2026** · ~90 gün

| Dönem | Tarih | Görev | Sorumlu |
|---|---|---|---|
| Hazırlık | Temmuz | Sunum hazırlama (demo + slaytlar) | Tüm ekip |
| Hazırlık | Ağustos | Mock jüri sorularına hazırlık | Ahmet Taha koordine |
| Hazırlık | Ağustos | Model demo arayüzü (opsiyonel) | Gizem + Ebrar |
| Finale | Ağustos–Eylül | **Yarışma Finalleri** | Tüm ekip |

---

### 🏆 FAZA 5 — TEKNOFEST Şanlıurfa
**30 Eylül – 4 Ekim 2026**

| Tarih | Görev |
|---|---|
| 30 Eylül – 4 Ekim | TEKNOFEST Şanlıurfa — Final sunumu |

---

## ✅ Bugün Toplantıdan Çıkacak Görevler

| # | Görev | Sorumlu | Deadline |
|---|---|---|---|
| 1 | Makale(lerini) oku + 5 soruluk özet hazırla | Herkes | 11 Mart |
| 2 | ClinVar + gnomAD veri erişimi sağla | Ali Andaç | 11 Mart |
| 3 | Bir sonraki toplantı tarihini belirle | Ahmet Taha | Bugün |
