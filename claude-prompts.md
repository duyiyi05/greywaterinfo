# Claude Code — Gri Su Veri Tabanı Promptları
**Versiyon:** 1.0 | **Tarih:** Mart 2026
**Kullanım:** Bu promptları Claude Code'a yapıştırın; veri tabanını sorgular, analiz üretir.

---

## PROMPT #1 — TEDARİKÇİ KARŞILAŞTIR

```
suppliers/by-region/asia/china.md dosyasındaki motorlu vana tedarikçilerinden
TOFINE, Kailing ve Valtec'i karşılaştır:

1. 100 adet fiyatı (USD)
2. MOQ (minimum sipariş)
3. Kalite / sertifikasyon
4. Garanti süresi
5. Teslimat süresi

Ardından 3 senaryo için öneri ver:
- 1–50 adet → hangi tedarikçi?
- 50–200 adet → hangi tedarikçi?
- 200+ adet → hangi tedarikçi?

Karşılaştırma tablosu + senaryo önerileri, Türkçe.
```

---

## PROMPT #2 — FUAR STRATEJİSİ

```
events/trade-fairs/ klasöründeki fuar verilerini kullanarak:

BÜTÇE: €20,000
HEDEF: Sistem tanıtımı + Parça tedariki
EKİP: 2 kişi

30 fuar arasından en iyi 3–5 fuarı seç ve şunları göster:
1. Maliyet dökümü
2. Beklenen ROI
3. Zaman çizelgesi (takvim)
4. Plan B (ana plan başarısız olursa)
5. Plan C (bütçe aşılırsa)

CEO'ya sunulacak formatta rapor, Türkçe.
```

---

## PROMPT #3 — FİYAT TASARRUF ANALİZİ

```
Mevcut durum: TOFINE motorlu vana, $35.80/adet, 200 adet/ay kullanım.

suppliers/by-region/asia/china.md'deki alternatif tedarikçilerden
en ucuz 3 seçeneği bul ve göster:

1. Birim fiyat farkı ($ ve %)
2. Aylık tasarruf ($)
3. Yıllık tasarruf ($)
4. Geçiş riski (MOQ, kalite, teslimat)
5. Öneri: hangi tedarikçiye geç, ne zaman?

Excel'e aktarılabilir tablo formatında, Türkçe.
```

---

## PROMPT #4 — CANTON vs IFAT KARAR

```
events/trade-fairs/fairs-2026.md'deki verileri kullanarak
Canton Fair (1–5 Mayıs) ve IFAT Munich (4–8 Mayıs) çakışmasını analiz et.

5 senaryo için karar ver:
1. Sadece parça tedariki amaçlıysa → hangisi?
2. Sadece sistem tanıtımı amaçlıysa → hangisi?
3. Bütçe kısıtlıysa (tek fuar) → hangisi?
4. Prestij / referans önemliyse → hangisi?
5. 2027'de her ikisine gitmeyi planlıyorsa → 2026'da hangisi?

Maliyet / fayda / ROI / lead karşılaştırması ile karar, Türkçe.
```

---

## PROMPT #5 — HAFTALIK ÖZET

```
Tüm veri tabanını (suppliers/ + events/) tara ve
bugün 22 Mart 2026 itibarıyla haftalık özet oluştur:

- Öne çıkan 3 gelişme / fırsat
- Tedarikçi durumu (yeni / güncellenmiş)
- Önümüzdeki 60 gün fuarlar
- Mevzuat / sertifikasyon hatırlatmaları
- Acil eylem gerektiren maddeler

Maksimum 1 sayfa, yöneticiye sunum formatı, Türkçe.
```

---

## KULLANIM NOTU

Bu promptlar `greywaterinfo/` deposundaki verilerle çalışır.
Veri güncellendikçe promptların çıktısı da otomatik güncellenir.
Yeni prompt eklemek için bu dosyayı düzenleyin.
