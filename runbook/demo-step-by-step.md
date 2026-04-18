# Demo Step-by-Step Script (90 Dakika)

Bu dosya, demoyu canli ortamda adim adim uygulamaniz icin hazirlandi.
Format: Her adimda "Ne yap", "Ne soyle", "Copilot prompt", "Beklenen cikti" bulunur.

## 0) Demo Oncesi Hazirlik (T-15 dk)

### Adim 0.1 - Ortam kontrolu
Ne yap:
- Repo klasorunun acik oldugunu kontrol et.
- Copilot Chat panelini ac.
- Asagidaki dosyalari solda pinle:
  - docs/process-overview.md
  - risk/risk-register.csv
  - issues/seed-issues.md
  - tests/uat-scenarios.md
  - prompts/demo-prompts.md

Ne soyle:
- "Bugun kod yazmadan surec kalitesini nasil arttirdigimizi gosterecegim."

Beklenen cikti:
- Katilimcilar demo akisinin kod disi surec odakli oldugunu net anlar.

### Adim 0.2 - Basari metriklerini acikla
Ne yap:
- metrics/demo-kpi-tracker.csv dosyasini ac.

Ne soyle:
- "Basariya sadece hizla degil kalite ile bakiyoruz: risk tamligi, issue olgunlugu ve UAT kapsami."

Beklenen cikti:
- Demonun olculebilir hedefleri netlesir.

## 1) Faz 1 - Problem Framing (0-15 dk)

### Adim 1.1 - Mevcut durumu goster
Ne yap:
- docs/process-overview.md dosyasini ac.
- KPI ve darbozazlari sesli oku.

Ne soyle:
- "Su an surec 18 is gunu suruyor ve rework orani %32. Ilk hedefimiz belirsizlikleri azaltmak."

Beklenen cikti:
- Herkesin uzlastigi tek bir problem tanimi olusur.

### Adim 1.2 - Hizli analiz promptu
Copilot prompt:
- "Bu surec metnini analiz et. Darbogazlari, rol belirsizliklerini, tekrarli adimlari ve olculemeyen noktalarini cikar. Sonucu tablo ver: Problem | Etki | Kok Neden | Onerilen Cozum | Hizli Kazanim."

Ne soyle:
- "Copilot'tan rapor degil, karar alinabilir cikti istiyoruz."

Beklenen cikti:
- 5 kolonlu net bir analiz tablosu.

## 2) Faz 2 - Surec Analizi ve TO-BE (15-35 dk)

### Adim 2.1 - AS-IS -> TO-BE donusumu
Ne yap:
- docs/as-is-to-be.md dosyasini ac.

Copilot prompt:
- "AS-IS surecini TO-BE modeline donustur. RACI mantiginda rol dagilimi ekle. Ilk 30 gun icin 5 aksiyon onceligi ver."

Ne soyle:
- "Hedefimiz guzel metin degil; sahipli, zamanli ve uygulanabilir plan."

Beklenen cikti:
- RACI benzeri rol dagilimi + 30 gun aksiyon listesi.

### Adim 2.2 - Ciktiyi standardize et
Ne yap:
- templates/output-template.md dosyasini ac.

Copilot prompt:
- "Urettigin surec analizini su formatta normalize et: Ozet | Varsayim | Risk | Aksiyon | Sorumlu | Termin | Insan Onayi Gerekir mi."

Beklenen cikti:
- Farkli ekiplerin ayni formatta ilerleyebilecegi standart cikti.

## 3) Faz 3 - Risk Analizi (35-55 dk)

### Adim 3.1 - Kritik riskleri cikar
Ne yap:
- risk/risk-register.csv dosyasini ac.

Copilot prompt:
- "Risk register verisini incele. Olasilik ve etkiye gore en kritik 5 riski sec. Her biri icin mevcut kontrol yeterliligini degerlendir ve ilave kontrol oner."

Ne soyle:
- "Risk listesi uzun olabilir; onceliklendirme yapmadan aksiyon alamayiz."

Beklenen cikti:
- Top 5 risk + kontrol boslugu + kontrol onerisi.

### Adim 3.2 - Risk kalitesi kontrolu
Copilot prompt:
- "Risk kayitlarinda dil tutarliligi, sahiplik netligi ve hedef tarih uygunlugunu kontrol et. Eksik alanlar icin duzeltme onerileri yaz."

Beklenen cikti:
- Veri kalitesi iyilestirme listesi (hangi satirda ne duzelmeli).

## 4) Faz 4 - Issue Kalitesi (55-75 dk)

### Adim 4.1 - Ham notlardan issue uret
Ne yap:
- issues/seed-issues.md dosyasini ac.

Copilot prompt:
- "Asagidaki ham notlari profesyonel GitHub issue formatina donustur. Her issue icin: Baslik, Baglam, Problem, Kabul Kriteri, Oncelik (MoSCoW), Sorumlu Rol, Termin."

Ne soyle:
- "Dogru issue, dogru ekipte daha hizli aksiyon demek."

Beklenen cikti:
- 10-12 adet olgun issue.

### Adim 4.2 - Sprint planina bagla
Copilot prompt:
- "Olusan issue listesini 3 sprinte dagit. Her sprint icin hedef, bagimlilik, risk ve cikti tanimi ver."

Beklenen cikti:
- Uygulanabilir 3 sprintlik roadmap.

## 5) Faz 5 - Test ve Kabul Kriterleri (75-85 dk)

### Adim 5.1 - UAT kapsamini genislet
Ne yap:
- tests/uat-scenarios.md dosyasini ac.

Copilot prompt:
- "Bu UAT setini genislet. Her senaryo icin en az 1 negatif ve 1 edge-case ekle. Beklenen sonucu olculebilir metrikle yaz ve test verisi ornegi ekle."

Ne soyle:
- "Test yazmadan guven olmaz; kabul kriteri olmadan test olmaz."

Beklenen cikti:
- Pozitif, negatif, edge-case kapsayan olculebilir UAT seti.

## 6) Faz 6 - Kapanis ve Yonetici Ozeti (85-90 dk)

### Adim 6.1 - Tek sayfalik ozet
Copilot prompt:
- "Tum ciktilari tek sayfalik yonetici ozetine cevir. Karar gerektiren 3 konu ve her konu icin 2 karar secenegi sun."

Ne soyle:
- "Copilot karar vermez; karar icin net secenek uretir."

Beklenen cikti:
- Yoneticinin hizli karar verecegi kisa ve net ozet.

### Adim 6.2 - KPI kapanis
Ne yap:
- metrics/demo-kpi-tracker.csv dosyasina demo sonunda gozlemsel measured degerleri gir.

Ne soyle:
- "Bu yaklasimi pilot ekipte 2 hafta denersek iyilesmeyi sayisal olarak gorecegiz."

Beklenen cikti:
- Demo etkisinin olculebilir kapanisi.

## 7) Soru Gelirse Hazir Cevaplar

Soru:
- "Bu ciktilar ne kadar guvenilir?"
Cevap:
- "AI oneri uretir, final karar ve onay insandadir. Bu nedenle her ciktiyi insan-onay adimi ile etiketliyoruz."

Soru:
- "Kuruma nasil uyarlariz?"
Cevap:
- "Ayni iskeleti koruyup sadece risk kategorileri, rol isimleri ve KPI hedeflerini kuruma ozel degistiririz."

Soru:
- "Bu teknik ekip olmadan uygulanir mi?"
Cevap:
- "Evet. Bu repo koddan bagimsiz surec artefaktlari ile tasarlandi."

## 8) Demo Sonrasi Aksiyon Listesi (Opsiyonel)

1. Ilk pilot sureci sec (1 ekip, 2 hafta).
2. Ayni prompt kutuphanesi ile yeniden calis.
3. KPI once/sonra degerlerini olc.
4. En yuksek etkiyi veren 3 promptu standartlastir.
5. Kurumsal "Copilot surec calisma rehberi"ni yayinla.
