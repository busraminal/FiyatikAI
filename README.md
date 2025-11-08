# 🚗 **FiyatikAI** — Akıllı İkinci El Araç Fiyat Tahmini Sistemi
Makine öğrenmesi tabanlı, kullanıcıdan alınan araç özelliklerine göre gerçekçi fiyat tahmini yapan web uygulaması.

> “Araç alırken kafadan fiyat çekme devri kapandı.”  
> FiyatikAI, gerçek veri + XGBoost modeli ile piyasa uyumlu sonuçlar üretir.

---

## ✨ Öne Çıkanlar
- 🔥 Gerçek veri (web scraping ile toplanmış ikinci el araç ilanları)
- 🎯 Eğitimli ML Modeli (XGBoost + karşılaştırmalı Linear & SVR)
- 🧩 Kolay Kullanım (Flask arayüzü + temiz form)
- ⚡ Anlık Tahmin (kullanıcı girişine göre gerçek zamanlı fiyat çıktısı)
- 🧱 Geliştirilebilir mimari (model yeniden eğitilebilir)

---

## 🧠 Teknik Mimari
| Katman | Teknoloji | Açıklama |
|------|-----------|----------|
| Veri | Pandas, NumPy | Web scraping → temizleme → feature engineering |
| Model | XGBoost, scikit-learn | Grid Search + R²/MAE ile değerlendirme |
| Arayüz | Flask, HTML, Bootstrap | Form tabanlı input + tahmin ekranı |

Model Kaydetme Formatı: **pickle (model.pkl)**

---

## 🚀 Kurulum ve Çalıştırma

```bash
git clone <repo-link>
cd FiyatikAI
pip install -r requirements.txt
python app.py
```

Tarayıcıda aç:
```
http://127.0.0.1:5000/
```

---

## 📁 Proje Yapısı

```
FiyatikAI/
│
├── app.py              # Flask ana uygulama
├── model.pkl           # Eğitimli ML modeli
├── data/
│   └── arac_verisi.csv # Web scraping ile elde edilen veri seti
├── templates/
│   └── index.html      # Arayüz
├── static/
│   └── style.css       # Tasarım düzenlemeleri
└── README.md
```

---

## 🎛️ Örnek Kullanım

Kullanıcı formda araç bilgilerini girer → Sistem fiyat tahmini verir.

**Çıktı:**
```
Tahmini Piyasa Fiyatı: 642.500 ₺
```

---

## 🧩 Geliştirme Yol Haritası

| Aşama | Durum | Not |
|------|------|-----|
| Model eğitimi + web arayüz | ✅ | Mevcut |
| Çoklu model karşılaştırma | ✅ | XGB > Linear > SVR |
| Piyasa trend API entegrasyonu | 🔜 | Sahibinden / Arabam API |
| Kullanıcı yorum/feedback sistemi | 🔜 | KVKK uyumlu |

---

## 🤝 Katkıda Bulunanlar
- **Büşra Mina AL**
- **Şevval ŞAHİN**

---

## 🛡️ Lisans
Bu proje **özel lisanslıdır**.  
Ticari veya akademik amaçlı kullanım için geliştirici onayı gereklidir.
