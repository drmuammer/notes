# Nedensel Çıkarım — DAG Odaklı Okuma Listesi

Epidemiyolojide nedensel çıkarım yöntemleri için kişisel okuma defterim. Odak: **Yönlendirilmiş Asiklik Grafikler (DAG)**.

---

## 📘 Temel Kitap

**Hernán MA, Robins JM. _Causal Inference: What If_. Boca Raton: Chapman & Hall/CRC, 2020.**

Alanın referans kitabı. PDF resmi olarak ücretsiz, sürekli güncelleniyor.

🔗 https://miguelhernan.org/whatifbook

R/Stata kod eşlikçisi: https://remlapmot.github.io/cibookex-r/

**Klinisyen için okuma sırası:**

- [ ] Bölüm 1–3 — Karşı-olgusal düşünce, randomizasyon, gözlemsel çalışmaların kavramsal temeli (matematiksiz)
- [ ] Bölüm 6–8 — DAG'ler, karıştırma, seçim yanlılığı
- [ ] Bölüm 12–13 — IPW (ters olasılık ağırlıklandırma) ve standardizasyon
- [ ] Bölüm 17 ve 22 — Target trial emülasyonu
- [ ] Geri kalanı — g-methods'a girdikten sonra ilgiye göre

> Not: Bölüm 2'yi tam anlamadan ilerleme; kitabın gerisi bu sezgiye yaslanıyor.

**İkincil kitap (daha kısa, DAG-merkezli giriş):**
Pearl J, Glymour M, Jewell NP. _Causal Inference in Statistics: A Primer_. Wiley, 2016.

**Popüler / kavramsal okuma:**
Pearl J, Mackenzie D. _The Book of Why_. Basic Books, 2018.

---

## 📑 DAG için Anahtar Makaleler

### Klasik temel
- [ ] **Greenland S, Pearl J, Robins JM (1999).** Causal diagrams for epidemiologic research. _Epidemiology_, 10(1):37–48.
  > Alanın temel taşı. Hâlâ en iyi giriş makalesi.

### Yapısal yaklaşım ve tuzaklar
- [ ] **Hernán MA, Hernández-Díaz S, Robins JM (2004).** A structural approach to selection bias. _Epidemiology_, 15(5):615–625.
  > Seçim yanlılığını DAG diliyle anlatan klasik.

- [ ] **Cole SR, Platt RW, Schisterman EF, et al. (2010).** Illustrating bias due to conditioning on a collider. _International Journal of Epidemiology_, 39(2):417–420.
  > Çarpıcı klinik örneklerle çarpıştırıcı (collider) tuzağı.

### Uygulamalı klinisyen-dostu
- [ ] **Tennant PWG, Murray EJ, Arnold KF, et al. (2021).** Use of directed acyclic graphs (DAGs) to identify confounders in applied health research: review and recommendations. _International Journal of Epidemiology_, 50(2):620–632.
  > Sistematik derleme; DAG'lerin pratikte nasıl yanlış kullanıldığını gösteriyor.

- [ ] **Lederer DJ, Bell SC, Branson RD, et al. (2019).** Control of confounding and reporting of results in causal inference studies. _Annals of the American Thoracic Society_, 16(1):22–28.
  > Klinik dergi raporlama rehberi olarak iyi.

---

## 🛠 Pratik Araçlar

| Araç | Kullanım |
|------|----------|
| **DAGitty** (dagitty.net) | Tarayıcıda DAG çizimi, otomatik adjustment seti çıkarma |
| **R `dagitty` paketi** | DAGitty'nin R entegrasyonu |
| **R `ggdag` paketi** | Yayına hazır DAG görselleştirmesi |

---

## 🎓 Kurslar

- [ ] **HarvardX "Causal Diagrams: Draw Your Assumptions Before Your Conclusions"** — Hernán'ın kendi kursu, ücretsiz, ~5 hafta. DAG'ler için en iyi yapılandırılmış giriş.
- **Coursera "A Crash Course in Causality"** (Roy, Penn State) — IPW ve eğilim skoru ağırlıklı.

---

## ✅ Pratik Egzersiz

Kendi alanından "yapamadığın bir RKÇ" sorusu seç (örn. _"X hastalığında erken vs geç tedavi başlama mortaliteyi etkiler mi"_), DAGitty'de DAG'ini çiz. Bu egzersiz tek başına bir aylık okumadan daha çok şey öğretir.

**Sorulacak sorular:**
1. Maruziyet (exposure) ve sonlanım (outcome) ne?
2. Hangi değişkenler ortak nedenler (karıştırıcı)?
3. Hangileri aracı (mediator) — bunlar için ayarlama yapma!
4. Hangileri çarpıştırıcı (collider) — bunlar için de ayarlama yapma!
5. DAGitty hangi minimum adjustment setini öneriyor?

---

## 📌 Sonraki Adımlar

DAG'leri sindirdikten sonra geçilecek başlıklar:

- **Target trial emülasyonu** — Matthews et al. (2022) BMJ makalesi iyi bir başlangıç
- **G-methods** — Naimi, Cole, Kennedy (2017) IJE makalesi üç yöntemi tek seferde anlatıyor
- **Eğilim skoru yöntemleri** — IPW, eşleştirme, stratifikasyon
- **Çift-sağlam tahmin (TMLE)** — modern hedeflenmiş öğrenme

---

_Son güncelleme: 2026-04_
