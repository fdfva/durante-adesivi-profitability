# DURANTE ADESIVI - PROFESYONEL KARLILIK HESAPLAMA VE ANALİZ SİSTEMİ

## 📋 Proje Özeti

Türkiye'de endüstriyel yapıştırıcı satışı yapan şirket için **gerçek kârlılık analizi** yapılmaktadır.

### 🎯 Amaç
- Ürün, müşteri, sipariş ve vade bazında **gerçek kârlılığı** hesaplamak
- Sadece "Satış Fiyatı - Alış Fiyatı" değil, **tüm maliyetleri** dahil etmek
- Yöneticinin doğru kararlar vermesine yardımcı olmak

---

## 📊 Excel Dosyası Yapısı (17 Sayfa)

### 1. **HAM VERİ** 📥
- Ürün bilgileri (kod, ad, grup)
- Müşteri bilgileri
- Satış siparişleri
- Nakliye ve gümrük giderleri
- Sabit giderler
- Kur bilgileri

### 2. **ÜRÜN MALİYETİ** 🏭
- Ürün kodu, adı, grubu
- Alış fiyatı (EUR)
- Alış tarihi
- KG başına maliyet
- Nakliye, gümrük, depolama
- **Toplam gerçek maliyet**

### 3. **ÜRÜN KARLILIK** 📈
- Satılan KG
- Satış fiyatı (TL/EUR)
- Brüt kâr
- Brüt kâr %
- Katkı payı
- Net kâr
- Net kâr %

### 4. **MÜŞTERİ KARLILIK** 👥
- Müşteri adı, kategori
- Toplam ciro
- Toplam KG
- Ortalama marj
- Finansman maliyeti
- Net kâr
- Müşteri durumu (🟢 iyi, 🟡 normal, 🔴 kötü)

### 5. **SİPARİŞ KARLILIK** 📦
- Sipariş no
- Müşteri
- Ürün
- Miktar
- Fiyat
- Maliyet
- Kâr

### 6. **VADE / FİNANSMAN** 💰
- Fatura tarihi
- Vade tarihi
- Tahsilat tarihi
- Vade gün sayısı
- Finansman maliyeti (yıllık %)
- Vade maliyeti (TL)
- Kâr (finansman sonrası)

### 7. **LOJİSTİK MALİYET** 🚚
- İtalya nakliye
- Ro-Ro, Kamyon
- Gümrük
- Antrepo, Liman
- Sigorta
- İç nakliye
- Depolama
- KG başına dağıtım

### 8. **SABİT GİDERLER** 🏢
- Personel
- Kira
- Elektrik, Telefon
- Araç, Yakıt
- Muhasebe, Yazılım
- Sigorta
- Ofis, Depo giderleri
- Toplam sabit gider (aylık)

### 9. **BAŞABAŞ** 📊
- Aylık sabit gider
- Ortalama katkı payı %
- Başabaş ciro
- Başabaş KG
- Başabaş satış miktarı

### 10. **İSKONTO ANALİZİ** 🎁
- Müşteri
- Liste fiyatı
- İskonto %
- Net fiyat
- İskonto etkisi
- Kaybedilen kâr

### 11. **KUR ANALİZİ** 💱
- Alış kuru (EUR/TL)
- Satış kuru
- Tahsilat kuru
- Kur farkı
- Kur riski

### 12. **SENARYO ANALİZİ** 🔄
- Senaryo A: Fiyat +%5
- Senaryo B: Fiyat -%5
- Senaryo C: Maliyet +%5
- Senaryo D: Kur ±%5
- Senaryo E: Vade +30 gün
- Senaryo F: Nakliye +%10

### 13. **ÜRÜN KARLILİK MATRİSİ** 🎨
- 🟢 ÇOK KARLI (%20+)
- 🟡 NORMAL (%10-%20)
- 🟠 DÜŞÜK KAR (%5-%10)
- 🔴 ÇOK DÜŞÜK (%0-%5)
- ⛔ ZARAR (-%0)

### 14. **MÜŞTERI SINIFLAMA** 📊
- En kârlı müşteriler
- En yüksek ciro
- En yüksek KG
- En yüksek marj
- En düşük marj
- Zarar ettiren
- Yüksek ciro, düşük kâr
- Uzun vade, düşük kâr

### 15. **VERİ KALİTESİ KONTROL** ⚠️
- Eksik alış fiyatı
- Eksik satış fiyatı
- Eksik kur
- Eksik vade
- Eksik nakliye
- Eksik müşteri
- Eksik KG

### 16. **SENARYO KARŞILAŞTIRMA** 📉
- Mevcut durum vs Senaryolar
- Ciro, Maliyet, Kâr, Kâr %
- Sensitivity analizi

### 17. **YÖNETİCİ DASHBOARD** 🎯
- 10 Kritik Sonuç
- KPI'lar
- Grafikler
- Aksiyon önerileri
- "Ne Yapmalıyız?" (5-10 somut adım)

---

## 📈 Ham Veri Örneği

### Ürünler
| Ürün Kodu | Ürün Adı | Grup | Alış Fiyatı EUR | KG |
|-----------|----------|------|-----------------|-----|
| P001 | Yapıştırıcı A | Genel | 8,50 | 1.000 |
| P002 | Yapıştırıcı B | Özel | 12,00 | 800 |
| P003 | Yapıştırıcı C | Teknik | 15,50 | 600 |

### Müşteriler
| Müşteri Adı | Kategori | Ortalama Vade (Gün) |
|-----------|----------|-------------------|
| Müşteri A | Büyük | 90 |
| Müşteri B | Orta | 60 |
| Müşteri C | Küçük | 30 |

### Satışlar
| Sipariş No | Müşteri | Ürün | KG | Satış Fiyatı TL | Fatura Tarihi |
|-----------|---------|------|-----|-----------------|---------------|
| S001 | Müşteri A | P001 | 200 | 50.000 | 01.01.2024 |
| S002 | Müşteri B | P002 | 150 | 48.000 | 05.01.2024 |
| S003 | Müşteri C | P003 | 100 | 35.000 | 10.01.2024 |

---

## 💡 Formül Örnekleri

### Brüt Kâr Formülü
```
Brüt Kâr = TL Satış Fiyatı - (Alış Maliyeti EUR × Kur) - Nakliye - Gümrük
```

### Finansman Maliyeti
```
Finansman Maliyeti = Satış Tutarı × Yıllık Oran × (Vade Gün / 365)
```

### Katkı Payı
```
Katkı Payı = Net Satış - Değişken Maliyetler
Katkı Payı % = Katkı Payı / Net Satış
```

### Net Kâr (Sabit Gider Dağıtılmış)
```
Net Kâr = Katkı Payı - (Sabit Giderler × Ürün Payı)
```

### Başabaş
```
Başabaş Ciro = Aylık Sabit Giderler / Ortalama Katkı Payı %
```

---

## 🚀 Kullanım Adımları

1. **HAM VERİ** sayfasına verilerinizi girin
2. Tüm formüller otomatik hesaplanacak
3. **YÖNETİCİ DASHBOARD** sayfasına bakın
4. Senaryo analizi yapın
5. Aksiyon alın

---

## 📞 İletişim

Herhangi bir soru için: `fdfva`

---

**Hazırlayan:** GitHub Copilot  
**Tarih:** 2024  
**Versiyon:** 1.0
