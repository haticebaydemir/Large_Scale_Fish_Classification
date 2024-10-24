
# Balık Türleri Sınıflandırma Projesi 
Bu proje, farklı balık türlerini sınıflandırmak için derin öğrenme teknikleri kullanarak bir model geliştirmeyi amaçlamaktadır. Python programlama dili ve TensorFlow ile Keras kütüphaneleri kullanılarak inşa edilmiştir.

## Proje Amacı 
Projenin temel amacı, balık türlerinin görüntülerini analiz ederek bu görüntülerin hangi türe ait olduğunu otomatik olarak belirlemektir. 

## Veri Seti 
Proje, Kaggle platformunda yer alan "A Large Scale Fish Dataset" veri setini kullanmaktadır. Bu veri seti, aşağıdaki 9 balık türüne ait toplam 9000 adet yüksek kaliteli PNG formatında görüntü içermektedir:

- Hourse Mackerel
- Black Sea Sprat
- Sea Bass
- Red Mullet
- Trout
- Striped Red Mullet
- Shrimp
- Gilt-Head Bream
- Red Sea Bream
Veri seti, her tür için yeterli örneklem sunarak modelin genel performansını artırmayı hedefler.

## Veri Setinin Özellikleri
- Format: PNG
- Toplam Görüntü Sayısı: 9000
Her Tür İçin Örnek Sayısı: Denge sağlanarak her türden yeterli sayıda örnek bulunmaktadır.

## Proje Yapısı 📁
Proje aşağıdaki aşamalardan oluşmaktadır:

1. **Gerekli Kütüphanelerin İçe Aktarılması**:

- NumPy, Pandas, Matplotlib, Seaborn gibi kütüphaneler veri analizi ve görselleştirme için kullanılır.
- TensorFlow ve Keras, derin öğrenme modelinin inşası için gereklidir.

2. **Veri Yükleme**:

- Balık türlerinin görüntüleri belirtilen dizinden yüklenir ve etiketlenir.
- Her görüntü için dosya yolu ve etiket bilgisi bir DataFrame yapısına aktarılır.

3. **Veri Ön İşleme***:

- Veri setinin analizi yapılır, eksik değerler kontrol edilir.
- Görüntülerin sayısal etiketleri dönüştürülür.

4. **Veri Setinin Ayırma**:

- Eğitim ve test veri setleri oluşturulur. Eğitim setinin %80'i, test setinin %20'si olarak ayrılır.

5. **Veri Artırma**:

- Eğitim verisi, görüntü işleme teknikleri (döndürme, kaydırma, yakınlaştırma) kullanılarak çeşitlendirilir. Bu, modelin genelleme yeteneğini artırır.

6. **Modelin Oluşturulması**:

- Konvolüsyonel Sinir Ağı (CNN) mimarisi tanımlanır.
- Modelde kullanılan katmanlar: Conv2D, MaxPooling2D, Flatten, Dense, Dropout, ve BatchNormalization.

7. **Modelin Eğitilmesi**:

- Model, eğitim veri setinde eğitilirken doğrulama veri seti ile sürekli olarak izlenir.
- Erken durdurma ve model kaydetme mekanizmaları ile modelin aşırı öğrenmesini önlemek için önlemler alınır.

8. **Sonuçların Analizi**:

- Model test edilir ve test kaybı, doğruluk oranı, karmaşıklık matrisi ve sınıflandırma raporları oluşturulur.


## Kullanılan Teknolojiler 
- **Python**: Projenin ana programlama dili.
- **TensorFlow & Keras**: Derin öğrenme modelinin geliştirilmesi için kullanılmıştır.
- **Pandas**: Veri analizi ve manipülasyonu için.
- **NumPy**: Sayısal işlemler  ve matris manipülasyonu için.
- **Matplotlib & Seaborn**: Veri görselleştirme ve grafik oluşturma için.
- **Scikit-learn**: Sınıflandırma raporları ve karmaşıklık matrisi oluşturma için.

# Model Performansı 
Model, eğitim ve test veri setleri üzerinde yüksek başarı göstermiştir. Elde edilen sonuçlar:

- **Test Kaybı**: 0.0151
- **Test Doğruluğu**: 99.61%

## Sınıflandırma Raporu
Modelin her bir sınıf için doğruluk, hatırlama (recall) ve F1 skoru gibi metrikleri içerir. Örneğin:

- Black Sea Sprat: Precision: 1.00, Recall: 1.00, F1-Score: 1.00
- Gilt-Head Bream: Precision: 1.00, Recall: 0.97, F1-Score: 0.98
Bu sonuçlar, modelin çoğu balık türünü yüksek doğrulukla sınıflandırabildiğini göstermektedir.


## Kaggle Linki 
Projenin detaylarına ve veri setine ulaşmak için: https://www.kaggle.com/code/haticebaydemir/large-scale-fish-classification

## İletişim 
Herhangi bir soru veya öneriniz varsa, lütfen benimle iletişime geçin. Proje ile ilgili geri bildirimleriniz benim için değerlidir.

E-posta: baydemirhatice@hotmail.com

Linkedln: https://www.linkedin.com/in/haticebaydemir/
