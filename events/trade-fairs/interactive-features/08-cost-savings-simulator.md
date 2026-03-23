# ÖZELLİK 8 — Maliyet Tasarruf Simülatörü
**Tedarikçi değişimi simülasyonu · Aylık/yıllık tasarruf hesabı**

---

## Simülasyon Parametreleri

### Mevcut Durum (Baseline)
| Ürün Kategorisi | Aylık Alım (adet) | Birim Fiyat (mevcut) | Aylık Maliyet |
|----------------|-------------------|---------------------|--------------|
| Motorlu vana (DN25) | 20 | €45 | €900 |
| Dalgıç pompa | 5 | €180 | €900 |
| UV sterilizatör | 10 | €95 | €950 |
| Bio filtre matı | 30 | €12 | €360 |
| PE tank (500L) | 4 | €280 | €1,120 |
| **TOPLAM** | — | — | **€4,230/ay** |

**Yıllık toplam (mevcut):** €50,760

---

## Senaryo A — Canton Tedarikçisi (Çin Direkt)

| Ürün Kategorisi | Yeni Fiyat | Tasarruf/Adet | Aylık Tasarruf | Yıllık Tasarruf |
|----------------|-----------|--------------|---------------|----------------|
| Motorlu vana (DN25) | €28 (-38%) | €17 | €340 | **€4,080** |
| Dalgıç pompa | €120 (-33%) | €60 | €300 | **€3,600** |
| UV sterilizatör | €58 (-39%) | €37 | €370 | **€4,440** |
| Bio filtre matı | €7 (-42%) | €5 | €150 | **€1,800** |
| PE tank (500L) | €180 (-36%) | €100 | €400 | **€4,800** |
| **TOPLAM** | — | — | **€1,560/ay** | **€18,720/yıl** |

**Geri ödeme süresi (Canton maliyeti $1,900):** 37 gün

---

## Senaryo B — Aquatech Avrupa Tedarikçisi

| Ürün Kategorisi | Yeni Fiyat | Tasarruf/Adet | Aylık Tasarruf | Yıllık Tasarruf |
|----------------|-----------|--------------|---------------|----------------|
| Motorlu vana (DN25) | €38 (-16%) | €7 | €140 | **€1,680** |
| Dalgıç pompa | €155 (-14%) | €25 | €125 | **€1,500** |
| UV sterilizatör | €80 (-16%) | €15 | €150 | **€1,800** |
| Bio filtre matı | €10 (-17%) | €2 | €60 | **€720** |
| PE tank (500L) | €240 (-14%) | €40 | €160 | **€1,920** |
| **TOPLAM** | — | — | **€635/ay** | **€7,620/yıl** |

**Geri ödeme süresi (Aquatech €3,100):** 147 gün (~5 ay)

---

## Senaryo C — Mix Strateji (Çin + Avrupa)

> Kritik/kalite gerektiren ürünler → Avrupa
> Yüksek hacimli/standart ürünler → Çin

| Ürün | Tedarikçi | Fiyat | Tasarruf/Yıl |
|------|----------|-------|-------------|
| Motorlu vana | Çin (Canton) | €28 | €4,080 |
| Dalgıç pompa | Avrupa (Aquatech) | €155 | €1,500 |
| UV sterilizatör | Çin (Canton) | €58 | €4,440 |
| Bio filtre matı | Çin (Canton) | €7 | €1,800 |
| PE tank | Çin (Canton) | €180 | €4,800 |
| **TOPLAM tasarruf** | — | — | **€16,620/yıl** |

**En iyi seçim:** Senaryo C — maksimum tasarruf + kalite güvencesi

---

## Karşılaştırma Özeti

| Senaryo | Yıllık Tasarruf | Fuar Maliyeti | Net Kazanç (Yıl 1) | Net Kazanç (Yıl 2+) |
|---------|----------------|--------------|-------------------|---------------------|
| A — Tam Canton | €18,720 | $1,900 | **€17,000** | €18,720 |
| B — Tam Avrupa | €7,620 | €3,100 | **€4,520** | €7,620 |
| C — Mix (önerilen) | €16,620 | €5,000 | **€11,620** | €16,620 |

---

## Hacim Bazlı Simülasyon

**Aylık alım artarsa tasarruf nasıl değişir?**

| Büyüme | Aylık Alım | Yıllık Tasarruf (C Senaryosu) |
|--------|-----------|-------------------------------|
| Mevcut | ×1 | €16,620 |
| +%50 büyüme | ×1.5 | €24,930 |
| +%100 büyüme | ×2 | €33,240 |
| +%200 büyüme | ×3 | €49,860 |

---

## Kalite Riski Faktörü

| Ürün | Çin Riski | Önlem | Ek Maliyet |
|------|----------|-------|-----------|
| Motorlu vana | Orta — elektrik arıza | CE sertifika iste | €0 |
| Pompa | Düşük — standart | ISO belge iste | €0 |
| UV sterilizatör | Düşük | UV gücü test et | €50/numune |
| Bio filtre | Çok düşük | Numune al, test et | €30/numune |
| PE tank | Çok düşük | Malzeme belgesi | €0 |
| **Toplam test maliyeti** | — | — | **€500** (bir kez) |

**Gerçek net tasarruf Yıl 1 (test dahil):** €11,120

---

## Simülasyon Nasıl Kullanılır

1. **Mevcut fiyatları güncelle** — baseline tablosunu doldurun
2. **Hacmi girin** — aylık/yıllık alım miktarınız
3. **Fuardan döndükten sonra** — yeni fiyatları girin
4. **Senaryo karşılaştır** — en iyi kombinasyonu seçin
5. **Yıllık net kazanç** = Tasarruf − Fuar maliyeti − Test maliyeti

---

*Bağlantı: `05-supplier-scorecard.md` · `04-roi-comparator.md`*
