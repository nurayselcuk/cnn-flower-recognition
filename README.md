
# 🌸 Derin Öğrenme ile Çiçek Sınıflandırma

Bu proje, transfer öğrenme (transfer learning) yaklaşımıyla farklı CNN modelleri kullanarak çiçek türlerini sınıflandırmayı amaçlamaktadır. TensorFlow ve Keras ile geliştirilmiş, Xception, InceptionV3 ve MobileNetV2 gibi güçlü modeller denenmiştir.

## 🎯 Proje Amacı

- Görsel veriler üzerinden çiçek türlerini sınıflandırmak
- Farklı CNN mimarilerini karşılaştırmak
- Precision, recall, f1 score ve confusion matrix gibi metriklerle performans değerlendirmek

## 🧠 Kullanılan Modeller

- ✅ Xception
- ✅ InceptionV3
- ✅ MobileNetV2

Her bir model:

- `include_top=False` ile önceden eğitilmiş katmanları kullanır.
- GlobalAveragePooling ve Dense layer eklenerek sınıflandırmaya uyarlanır.
- Eğitim ve validasyon sonuçları görselleştirilir.

## 📁 Veri Seti

- Klasör yapısı: `/flower/cicekler/`
- Alt klasörler her bir çiçek türünü temsil eder.
- Train/validation/test olarak `ImageDataGenerator` kullanılarak ayrılır.

## ⚙️ Kullanılan Kütüphaneler

- `TensorFlow / Keras`
- `scikit-learn`
- `NumPy`
- `Matplotlib & Seaborn`

## 📈 Performans Metrikleri

- Doğruluk (Accuracy)
- Precision, Recall, F1 Score (weighted ortalama ile)
- Confusion Matrix (sınıflar arası karışıklık görselleştirilir)

## 🚀 Kullanım

1. Google Colab veya Jupyter Notebook ile açın
2. `data_dir` yolu kendi veri setinize göre değiştirin
3. Notebook hücrelerini sırasıyla çalıştırın

```python
data_dir = '/content/drive/MyDrive/flower/cicekler'
```

## 🖼️ Çıktılar

- Eğitim doğruluğu
- Test doğruluğu
- Confusion Matrix görselleştirmeleri
- Precision / Recall / F1 değerleri

## 📌 Notlar

- Giriş görüntü boyutları: `224x224` ya da `299x299` (modele göre)
- `class_mode='categorical'` olarak ayarlanmış (çok sınıflı)
- Model karşılaştırması yapılmıştır
