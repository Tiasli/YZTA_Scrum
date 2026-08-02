# Passport Visa Checker 🌍✈️

## Takım İsmi
51. Bölge

**Passport Visa Checker**, karmaşık ve dağınık vize bilgilerini doğrulayarak tek bir interaktif harita üzerinde sunan web tabanlı bir uygulamadır. Kullanıcıların seçtiği pasaporta göre tüm dünyanın vize durumunu saniyeler içinde görselleştirir.

---

## Öne Çıkan Özellikler

- **Anlık Görselleştirme:** Pasaport seçimi yapıldığı anda dünya haritası vize durumlarına göre 5 farklı kategoride renklenir.
- **Sıfır Sürtünme:** Hesap oluşturma, kurulum veya bekleme süresi yok. Doğrudan tarayıcı üzerinden çalışır.
- **Detaylı Bilgi Paneli:** Seçilen ülke için:
  - İzin verilen maksimum kalış süresi (gün)
  - Gerekli belgeler (Required Documents)
  - Son dönem vize değişiklikleri (Recent Visa Changes)
  - Ülkeye özel seyahat notları (Travel Notes)
- **Dinamik Yeniden Hesaplama:** Farklı bir pasaport seçildiğinde 199 ülkenin tümü için vize durumları anında yeniden hesaplanır.
- **Sıfır Maliyet & Yüksek Hız:** Backend ve veritabanı bağımlılığı olmayan tamamen statik ve performanslı mimari.
---

## Hedef Kitle

-  **Bağımsız Seyahat Edenler**
-  **Dijital Göçebeler (Digital Nomads)**
-  **Rota Planlayan Öğrenciler**

---

## Vize Kategorileri

Harita üzerinde her renk farklı bir vize durumunu temsil eder:

1. **Vizesiz (Visa-Free)**
2. **Kapıda Vize (Visa on Arrival)**
3. **E-Vize (e-Visa)**
4. **Elektronik Seyahat İzni (eTA)**
5. **Vize Zorunlu (Visa Required)**

---

## Teknik Mimari & Veri Güvenilirliği

Sistemin en temel önceliği doğru ve güvenilir bilgi sunmaktır.

### Veri Doğrulama Hattı (Data Pipeline)
- **Veri Kaynağı:** Güncel vize verileri *Passport Index* kaynağından çekilir.
- **CI/CD Doğrulama:** GitHub Actions üzerinde çalışan otomatik bir doğrulama hattı, veriyi yapısal kontrolden geçirir ve SHA-256 özetini oluşturur.
- **Client-Side Integrity Check:** Tarayıcı veriyi yüklerken SHA-256 özetini yeniden hesaplar ve doğrular. Eşleşmeyen veya tahrif edilmiş veri tespit edilirse sistem yanlış bilgi vermek yerine kendini kapatır.

### Ön Yüz & Güvenlik
- **Harita & Görselleştirme:** Leaflet ve TopoJSON mimarisi kullanılarak sınırlar yerel olarak hızlıca çizdirilir.
- **Güvenlik Sıkılaştırması:** Content Security Policy ve Subresource Integrity kontrolleri aktif olarak kullanılır.
- **Mimari:** Sıfır backend, sıfır veritabanı. Statik yapısı sayesinde çevrimdışıya yakın çalışma hızı ve sıfıra yakın barındırma maliyeti sağlar.

---

## Takım (51. Takım)

- **Aslı** 
- **Berkin** 
- **Melisa** 

---
