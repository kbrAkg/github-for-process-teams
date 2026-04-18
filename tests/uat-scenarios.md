# UAT Senaryo Seti

## Senaryo 1: Dusuk Riskli Tedarikci Hizli Gecis
- On kosul: Tum zorunlu alanlar dolu, ulke dusuk risk.
- Adimlar:
  1. Talep formu acilir.
  2. Otomatik on kontrol tamamlanir.
  3. Risk skoru hesaplanir.
  4. Hizli onay hatti ile kayit kapanir.
- Beklenen sonuc: 2 is gunu icinde onboarding tamamlanir.
- Basarisizlik sinyali: Bir adim 48 saatten fazla bekler.

## Senaryo 2: Yuksek Riskli Ulke Ek Kontrol
- On kosul: Ulke risk seviyesi yuksek olarak isaretli.
- Adimlar:
  1. Talep formu acilir.
  2. Sistem yuksek risk kontrol adimini zorunlu kilar.
  3. Compliance ek kanit ister.
  4. Legal ikinci goz kontrolu yapar.
- Beklenen sonuc: Ek kontrol adimlari tamamlanmadan surec ilerlemez.
- Basarisizlik sinyali: Ek kontrol olmadan ERP acilisi yapilir.

## Senaryo 3: Eksik Evrakla Surecin Durmasi
- On kosul: KYC belgesinden biri eksik.
- Adimlar:
  1. Talep kaydi acilir.
  2. Evrak kontrol adimi calisir.
  3. Sistem eksik belgeyi listeler.
- Beklenen sonuc: Eksik belge tamamlanana kadar onay akisi baslamaz.
- Basarisizlik sinyali: Eksik belge varken hukuk/finans onayi baslar.

## Senaryo 4: Red Sonrasi Yeniden Basvuru
- On kosul: Tedarikci onceki kayitta red almis.
- Adimlar:
  1. Yeni basvuru acilir.
  2. Sistem onceki karar kaydini getirir.
  3. Bekleme suresi kuralini uygular.
- Beklenen sonuc: Politika disi yeniden basvuru engellenir.
- Basarisizlik sinyali: Kural disi kayit kabul edilir.

## Senaryo 5: Audit Izi Tamligi
- On kosul: Bir onboarding vakasi tum adimlardan gecmis.
- Adimlar:
  1. Karar gecmisi raporu cagrilir.
  2. Tum onay, red, eskalasyon kayitlari listelenir.
- Beklenen sonuc: Denetim icin gerekli tum kayitlar tek raporda gorulur.
- Basarisizlik sinyali: Gerekce veya onay sahibi alanlari bos gelir.

## Copilot Gorevi
Bu seti genislet:
- Her senaryo icin en az 1 negatif ve 1 edge-case ekle.
- Beklenen sonucu olculebilir metrikle yaz.
- Her senaryoya test verisi ornegi ekle.
