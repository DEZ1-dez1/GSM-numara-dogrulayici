# 📱 Türkiye GSM & Telefon Numarası Doğrulama Aracı

![Lisans: MIT](https://img.shields.io/badge/Lisans-MIT-blue.svg)
![PR'lar Açık](https://img.shields.io/badge/PR'lar-kabul_edilir-brightgreen.svg)
![Vanilla JS](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)

Türkiye'deki tüm GSM operatörlerinin (Turkcell, Vodafone, Türk Telekom, Netgsm vb.) ve sabit hatların formatını doğrulayan, numaranın ilk tahsis edildiği orijinal operatör bloğunu anlık olarak tespit eden açık kaynaklı web uygulaması.

---

## 📌 Bu Araç Ne İşe Yarar?

Yazdığınız telefon numarasının eksiksiz ve BTK standartlarına uygun olup olmadığını anında kontrol eder:

1. **Format ve Uzunluk Doğrulama:** Numaranın `05XX XXX XX XX` standartlarında, tam 11 haneli ve "05" ile başlayıp başlamadığını denetler.
2. **Orijinal Operatör Tespiti:** Numarayı oluşturan ilk 3 haneli kök bloktan (Prefiks) numaranın ilk olarak hangi operatörden çıkarıldığını anlık olarak gösterir.
3. **Akıllı Biçimlendirme:** Siz tuşladıkça telefon numarasını otomatik olarak okunabilir boşluklu formata getirir.

---

## ✨ Öne Çıkan Özellikler

- **BTK Operatör Blokları Entegrasyonu:**
  - 🟡 **Turkcell** (`530-539`, `561`)
  - 🔴 **Vodafone** (`540-549`)
  - 🔵 **Türk Telekom** (`501`, `505-507`, `551-555`, `559`)
  - 🟢 **Netgsm & Sanal Operatörler** (`510`, `516`)
- **Numara Taşınabilirliği (NPT) Bilgilendirmesi:** Sistem, numaranın ilk alındığı operatörü gösterir. (Not: Türkiye'de numara taşıma sistemi olduğu için hat başka bir operatöre taşınmış olabilir).
- **%100 İstemci Taraflı (Client-Side) Güvenlik:** Hiçbir numara sunucuya gönderilmez veya kaydedilmez. Tüm işlemler tamamen tarayıcınızda gerçekleşir.
