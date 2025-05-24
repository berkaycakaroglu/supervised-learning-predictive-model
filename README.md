# Gözetimli Öğrenme ile Tahmin Modeli

Bu proje, **Akbank Makine Öğrenmesi Bootcamp 2025** kapsamında geliştirilmiş olup, gözetimli öğrenme teknikleri kullanılarak gerçekleştirilmiştir. Veri seti üzerinde hem keşifsel veri analizi (EDA) yapılmış, hem de çeşitli makine öğrenmesi algoritmaları kullanılarak sınıflandırma problemleri çözülmüştür.

---

## 🔍 Giriş

Projede kullanılan veri seti: Formula 1 World Championship (1950–2024)
Veri seti, 1950 yılından günümüze kadar yapılmış Formula 1 yarışlarına ait kapsamlı bilgileri içermektedir. 14 farklı CSV dosyasından oluşur ve sürücüler, takımlar, yarış sonuçları, tur zamanları, pit stop verileri gibi çeşitli detaylar barındırır.

Problem türü: Sınıflandırma / Regresyon
Hedef değişken: positionOrder, milliseconds, veya qualifying time (problem tanımına göre değişir)

Bu projede:
- Veri analizi ve görselleştirmeler yapılmıştır.
- Veri ön işleme adımları (eksik değer analizi, kategorik değişken dönüştürmeleri, ölçekleme vb.) gerçekleştirilmiştir.
- Birden fazla model eğitilmiş ve performansları karşılaştırılmıştır.
- En iyi sonuç veren model hiperparametre ayarlaması ile optimize edilmiştir.

---

## 📊 Kullanılan Algoritmalar

- Lojistik Regresyon
- Karar Ağaçları (Decision Tree)
- KNN (K-Nearest Neighbors)
- SVM (Support Vector Machine)

Bonus olarak ayrıca:
- k-Means ile gözetimsiz öğrenme uygulanmıştır. (isteğe bağlı)
- Proje Streamlit ile deploy edilmiştir. (isteğe bağlı)

---

## 📈 Metrikler ve Yorumlar

Seçilen modelin değerlendirilmesinde şu metrikler kullanılmıştır:

**Sınıflandırma:**
- Doğruluk (Accuracy)
- Kesinlik (Precision)
- Duyarlılık (Recall)
- F1 Skoru
- Karışıklık Matrisi

**Regresyon ise:**
- Ortalama Mutlak Hata (MAE)
- Ortalama Kare Hata (MSE)
- R-Kare (R²)

Modelin elde ettiği doğruluk oranı: **[%.xx]**  
Model çıktıları ve bu çıktılara dair analizler notebook dosyasında markdown hücreleri ile açıklanmıştır.

---

## 🖥️ Ekler

- Streamlit ile arayüz geliştirildi ve model deploy edildi.
- GPU destekli kütüphaneler ile (cuML, RAPIDS, vb.) eğitim tekrarlanarak hız karşılaştırması yapıldı.

---

## 🎯 Sonuç ve Gelecek Çalışmalar

Bu proje ile gözetimli öğrenme süreçleri uçtan uca deneyimlenmiştir. Gelecekte:

- Daha büyük ve dinamik veri kaynaklarıyla çalışılabilir,
- Modelin başarımı artırmak için ensemble yöntemler (Random Forest, XGBoost) denenebilir,
- Model bir REST API ile entegre edilerek farklı uygulamalarda kullanılabilir,
- Proje mobil uygulama arayüzü ile sunulabilir.

---

## 🔗 Kaggle Notebook Linkleri

- [📌 Supervised Öğrenme Notebook (Kaggle)](https://www.kaggle.com/code/kullaniciadi/notebook-adresiniz)
- [📌 (Opsiyonel) GPU ile Hızlandırılmış Çalışma](https://www.kaggle.com/code/kullaniciadi/gpu-ile-ml)
- [📌 (Opsiyonel) Deploy Edilmiş Proje](https://github.com/kullaniciadi/proje-linki)
