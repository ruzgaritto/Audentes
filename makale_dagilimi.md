# 📖 Makale Okuma Görevlendirme Tablosu — Audentes

**Proje:** Teknofest Sağlıkta Yapay Zeka — Missense Varyant Patojenisitesi  
**Güncelleme:** 9 Mart 2026

---

## 👥 Kişi Bazlı Detaylı Liste

---

### 👤 Ahmet Taha Çelik — Klinik Bağlam & Genomik Veri

| # | Makale | Yıl | Dergi | Ücretsiz Link |
|---|---|---|---|---|
| 1 | Richards et al. — *Standards and guidelines for the interpretation of sequence variants* (ACMG/AMP) | 2015 | Genetics in Medicine | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4544753/ |
| 2 | Karczewski et al. — *The mutational constraint spectrum from 141,456 humans* (gnomAD v2) | 2020 | Nature | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7334197/ |
| 🆕 | Chen et al. — *A genomic mutational constraint map using 76,156 human genomes* (gnomAD v4) | 2024 | Nature | https://www.biorxiv.org/content/10.1101/2022.03.20.485034 |

**Odak:** "Neden bazı varyantlar patojenik?" sorusunun klinik ve popülasyon genetiği cevabı.  
`gnomAD_AF` özelliğini ve `o/e ratio` metriğini derinlemesine anla.

---

### 👤 Ali Andaç Erdaş — Ensemble & Klasik ML Yöntemleri

| # | Makale | Yıl | Dergi | Ücretsiz Link |
|---|---|---|---|---|
| 1 | Ioannidis et al. — *REVEL: An Ensemble Method for Predicting the Pathogenicity of Rare Missense Variants* | 2016 | AJHG | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5065685/ |
| 2 | Alirezaie et al. — *ClinPred: Prediction Tool to Identify Disease-Relevant Nonsynonymous SNVs* | 2018 | AJHG | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6174280/ |
| 🆕 | *(Anonim)* — *Disease- and gene-specific deep learning for pathogenicity prediction of rare missense variants in cancer predisposition genes* | 2026 | BioData Mining | *(DOI yakında — ResearchGate üzerinden erişilebilir)* |

**Odak:** "Neden kendi modelimizi kuruyoruz, REVEL/ClinPred neden yetmez?" sorusunu cevaplayabilmek.  
Ensemble stratejisi, VUS (belirsiz varyant) problemi ve limitler.

---

### 👤 Gizem Öksüz — Derin Öğrenme & AlphaFold Tabanlı Yöntemler

| # | Makale | Yıl | Dergi | Ücretsiz Link |
|---|---|---|---|---|
| 1 | Cheng et al. — *Accurate proteome-wide missense variant effect prediction with AlphaMissense* | 2023 | Science | https://www.science.org/doi/10.1126/science.adg7492 |
| 🆕 | Öztürk et al. — *PreMode: predicts mode-of-action of missense variants by deep graph representation learning* | 2025 | Nature Communications | https://doi.org/10.1038/s41467-025-62318-4 |

**Odak:** AlphaMissense şu anki alan standardı — tüm performans metriklerini öğren.  
Jüri "sizin modeliniz AlphaMissense'e kıyasla ne kadar iyi?" diye soracak.  
PreMode'daki GNN mimarisi yeni yaklaşım için ilham kaynağı.

---

### 👤 Ebrar Yılmaz — Protein Dil Modelleri

| # | Makale | Yıl | Dergi | Ücretsiz Link |
|---|---|---|---|---|
| 1 | Meier et al. — *Language models enable zero-shot prediction of the effects of mutations on protein function* (ESM-1v) | 2021 | NeurIPS | https://openreview.net/forum?id=uSj3Nf2Pgq |
| 2 | Lin et al. — *Evolutionary-scale prediction of atomic-level protein structure with a language model* (ESM-2) | 2023 | Science | https://www.biorxiv.org/content/10.1101/2022.07.20.500902v3 |
| 🆕 | DIVA — *Disease-specific variant pathogenicity prediction using multimodal biomedical language models* | 2025 | bioRxiv | https://www.biorxiv.org/content/10.1101/2025.09.09.675184 |

**Odak:** ESM-1v ve ESM-2 ikisi de Meta AI'dan protein dil modeli — farkını anla: ESM-1v fonksiyon tahminine, ESM-2 yapı tahminine odaklı.  
DIVA, ESM çıktılarını multimodal bağlamda (hastalık metinleri + contrastive learning) nasıl kullandığını gösteriyor.

---

### 👤 Songül Sevinti — Skor Tabanlı Yöntemler & Yapısal Entegrasyon

| # | Makale | Yıl | Dergi | Ücretsiz Link |
|---|---|---|---|---|
| 1 | Rentzsch et al. — *CADD: predicting the deleteriousness of variants throughout the human genome* | 2019 | NAR | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6323946/ |
| 🆕 | Schubach et al. — *CADD v1.7: Using protein language models, regulatory CNNs and other nucleotide level scores* | 2024 | NAR | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10767980/ |
| 🆕 | Danner et al. — *Utilizing protein structure graph embeddings to predict the pathogenicity of missense variants* | 2025 | NAR Genomics | https://academic.oup.com/nargab/article/7/3/lqaf097/8209846 |

**Odak:** CADD v1.7 içinde ESM-1v var → ESM–CADD bağlantısını kur.  
Graph embedding + XGBoost pipeline formatını anla; doğrudan projeye uygulanabilir.

---

## 📝 Makale Özet Formatı

Her kişi okuduğu makale için aşağıdaki 5 soruyu yanıtlayacak:

1. **Problem ne?** — Makale hangi sorunu çözüyor?
2. **Hangi veri kullanıldı?** — Eğitim/test verisi ne?
3. **Hangi yöntem/model kullanıldı?** — Mimari veya algoritma ne?
4. **Elde ettikleri F1/AUC/Accuracy ne?** — Sayısal performans metrikleri?
5. **Bizim projemizle ilişkisi nedir?** — Bu makale projemize nasıl katkı sağlar?
