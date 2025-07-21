# 🎓 Bitirme Projesi 2 – Veri Analizi (Power BI)

## 👩‍💻 Proje Sahibi: Sena Gürkan  
📅 Tarih: 21 Temmuz 2025  
🎯 Marka: **ETİ**  
📊 Araç: Microsoft Power BI  
📁 Veri Kaynağı: Kullanıcı, Sipariş, Ürün, Adres ve Bölge verileri (CSV)

🔗 [Rapor Dosyaları ve PDF Görseller (Google Drive)](https://drive.google.com/drive/folders/1Y-8OFAs8hsY57-zNRigI3GX0j049X4sk?usp=sharing)

---

## 🔍 Proje Amacı

Bu proje kapsamında, ETİ markasına ait müşteri, sipariş ve ürün satış verileri analiz edilerek:

- Verinin dönüştürülmesi  
- Modelleme yapılması  
- Power BI üzerinde gelişmiş görselleştirme uygulanması  
- İş biriminin analiz ihtiyaçlarını karşılayacak raporların oluşturulması amaçlanmıştır.

---

## 💻 Kullanılan Teknolojiler

- Power BI Desktop  
- DAX (Data Analysis Expressions)  
- Veri Modelleme  
- Veri Temizleme ve Dönüştürme  
- Görselleştirme Teknikleri  

---

## 🧱 Kullanılan Veri Setleri

| Tablo Adı        | Açıklama                                   |
|------------------|---------------------------------------------|
| kullanıcılar     | Müşteri bilgileri                           |
| adres            | Kullanıcıların adres bilgileri              |
| ürünler          | Ürün bilgileri (kategori, marka, fiyat vs)  |
| sipariş          | Sipariş temel bilgileri (tarih, adres vs)   |
| siparisdetay     | Sipariş detay bilgileri                     |
| bölgeler         | Şehir ve bölge eşleştirme tablosu           |

---

## 🛠️ Yapılan Dönüşümler ve Hazırlıklar

Veri üzerinde birçok dönüşüm ve hazırlık işlemi gerçekleştirilmiştir. Bunlardan bazıları:

- Doğum tarihinden yaş hesaplanması, cinsiyetin metne çevrilmesi  
- Yeni sütunların türetilmesi (yaş grubu, gün türü, saat bilgisi vb.)  

Ayrıca kategori verileri sadeleştirilmiş, ETİ markasına özel tablo filtrelenmiş ve tüm sayısal tipler uygun biçimlere dönüştürülmüştür.

---

## 🔗 Modelleme İlişkileri

- `kullanıcılar[ID]` → `sipariş[USERID]`  
- `sipariş[ID]` → `siparisdetay2[ORDERID]`  
- `ürünler[ID]` → `siparisdetay2[ITEMID]`  
- `adres[ID]` → `sipariş[ADDRESSID]`  
- `bölgeler[SehirAd]` → `adres[CITY]`  

---

## 📊 Rapor Sayfaları

### 🟩 1. Giriş Sayfası

Proje amacı, açıklamalar ve sayfalar arası geçiş butonları yer alır. Teşekkür bölümü de bu sayfada sunulmuştur.

### 📘 2. Özet Sayfa

Genel metrikler (toplam satış, ciro, sipariş vb.) kartlarla gösterilmiştir.
Satışların günlere, saatlere ve bölgelere göre dağılımı grafiklerle sunulmuştur.

### 🧑‍🤝‍🧑 3. Müşteri Perspektifi

Müşteri demografisi ve davranışları analiz edilmiştir.
Cinsiyete, yaş grubuna, şehirlere göre dağılımlar ve İstanbul’daki top 10 müşteri tablolarla gösterilmiştir.

### 🛒 4. Kategori Perspektifi

Kategori bazında performans değerlendirilmiştir.
En çok satış yapılan ve ciro getiren kategoriler kartlarla; satış oranları pasta grafikle; İstanbul’daki yetişkin müşterilere ait ciro dağılımı ise ağaç haritasıyla görselleştirilmiştir.

---

## 🗂️ Teslim Formatı

- `ETI_Satis_Analizi_SenaGurkan.pbix` → Power BI dosyası (Drive Linkinde) 
- `ETI_Satis_Raporu_SenaGurkan.pdf` → Grafiksel çıktı  
- `README.md` → Bu döküman  

---

## 🙏 Teşekkür

Bu proje, **Kız Başına Veri Analizi Bootcamp** kapsamında hazırlanmıştır.  
Eğitim süreci boyunca desteklerini esirgemeyen başta **Mehmet Yalçın** ve **Mert Alabaş** olmak üzere, tüm eğitmenlere, organizasyon ekibine ve ekip arkadaşlarıma teşekkür ederim.

---
