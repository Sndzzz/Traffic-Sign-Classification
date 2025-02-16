# Traffic-Sign-Classification  

Bu proje, derin öğrenme kullanarak trafik işaretlerini sınıflandırmayı amaçlamaktadır.  
Google Colab üzerinde CNN (Convolutional Neural Network) modeli ile eğitilmiştir.  

---

## Proje Açıklaması  
Bu çalışmada Almanya Trafik İşaretleri Veri Seti (GTSRB) kullanılarak trafik işaretlerini sınıflandıran bir model geliştirilmiştir.  
✅ Google Colab ortamında Kaggle API ile veri seti çekildi.  
✅ Görseller işlenerek (30x30) boyutuna getirildi ve normalize edildi.  
✅ CNN modeli eğitildi ve test doğruluğu hesaplandı. 
✅ Modelin performansı Accuracy & Loss grafikleri ile analiz edildi.  
✅ Test verileriyle modelin tahmin yapması (Inference) sağlandı.  

---

## Kullanılan Teknolojiler  
- Python 3.9+ 
- TensorFlow / Keras  
- Matplotlib / Pandas / NumPy 
- Scikit-learn 
- Google Colab  

---

## Kullanılan Veri Seti  
Bu projede GTSRB - German Traffic Sign Recognition Benchmark veri seti kullanılmıştır.  
-Veri Seti Linki: [Kaggle - GTSRB Dataset](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)  

Bu veri seti toplamda 43 farklı trafik işareti sınıfı içermektedir ve modelimiz bu sınıfları doğru şekilde tahmin edebilmektedir.  

---

## Kurulum ve Kullanım  
Eğer kodları kendi bilgisayarında çalıştırmak istiyorsan, aşağıdaki adımları takip et:  

### 1️⃣ Gerekli Kütüphaneleri Yükle 
```bash
pip install tensorflow numpy pandas matplotlib opencv-python tqdm keras scikit-learn Pillow
```
### 2️⃣ Google Colab’de Çalıştırma
Projeyi Google Colab üzerinde çalıştırmak için:

-Google Drive'ı bağla
-Kaggle API ile veri setini çek
-Kodları çalıştırarak modeli eğit ve test et

## Model Performansı  
Model eğitim ve test seti üzerinde doğrulama yapıldıktan sonra aşağıdaki yaklaşık sonuçlar elde edilmiştir:  

-Test Doğruluğu (yaklaşık): %98.5  
-Eğitim Kaybı (yaklaşık): %0.10  

Bu değerler eğitim sürecinde gözlemlenen doğrulama (validation) doğruluğu ve kayıp (loss) grafiklerinden tahmini olarak alınmıştır.

## Modelin Tahmin Yapması (Inference)
Eğitilen modelin gerçek bir trafik işareti üzerinde tahmin yapmasını test etmek için aşağıdaki kodu çalıştırabilirsiniz:
```bash
image_path = "Test/00005.png"
predict_image(model, image_path, class_labels)
```
Örnek çıktı:
```
Tahmin Edilen Sınıf: 16  
Olasılık Değeri: 0.9999  
```

## Lisans & Kaynaklar
GTSRB Veri Seti: Almanya Trafik İşaretleri Tanıma Veri Seti
Referanslar:
-Traffic Sign Recognition using Deep Neural Networks
-[Kaggle - Traffic Sign Dataset](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)  

## İletişim
Eğer proje hakkında sorularınız varsa benimle iletişime geçebilirsiniz:
-> GitHub:[GitHub Hesabım](https://www.github.com/Sndzzz)
-> E-posta: sudenazsenbay@gmail.com
-> LinkedIn: [LinkedIn Profilim](https://www.linkedin.com/in/sudenaz-şenbay)
