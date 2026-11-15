# Fashion-MNIST CNN Sınıflandırma Projesi

## Proje Hakkında
Bu projede Fashion-MNIST veri seti kullanılarak
Evrişimsel Sinir Ağı (CNN) modeli ile giysi görüntülerinin
10 sınıfa ayrılması amaçlanmıştır.

## Kullanılan Teknolojiler
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Veri Seti
Fashion-MNIST veri seti 28x28 piksel boyutunda,
gri tonlamalı 70.000 görüntüden oluşur.
10 farklı giysi sınıfı bulunmaktadır.

- Eğitim verisi: 54.000 görüntü
- Doğrulama verisi: 6.000 görüntü
- Test verisi: 10.000 görüntü

## Model Mimarisi
- Conv2D: 32 filtre
- MaxPooling2D
- Conv2D: 64 filtre
- MaxPooling2D
- Conv2D: 128 filtre
- GlobalAveragePooling2D
- Dropout: 0.30
- Dense: 10 çıkış sınıfı

## Deney Ayarları
- Rastgelelik tohumu: 42
- Deney sayısı: 3
- Epoch: 10
- Batch size: 128
- Optimizasyon: Adam
- Öğrenme oranı: 0.001
- Kayıp fonksiyonu: Sparse Categorical Crossentropy

## Dosyalar
- CNN_Fashion_MNIST_Odevi.ipynb: Model ve deney kodları
- requirements.txt: Gerekli Python kütüphaneleri
- PNG dosyaları: Grafikler ve şekiller
- CSV dosyaları: Deney tabloları

## Kurulum
Gerekli kütüphaneleri yüklemek için:

    pip install -r requirements.txt

## Çalıştırma
Notebook dosyasını Google Colab veya Jupyter Notebook
üzerinde açarak hücreleri sırasıyla çalıştırabilirsiniz.

## Veri Seti Kaynağı
Fashion-MNIST:
https://github.com/zalandoresearch/fashion-mnist
