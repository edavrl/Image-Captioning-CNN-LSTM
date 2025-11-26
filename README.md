# Image Captioning with CNN & LSTM

![Python](https://img.shields.io/badge/Python-3.10-3776AB)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-FF6F00)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-D00000)
![Status](https://img.shields.io/badge/Status-Completed-success)

## Project Description
This project implements an image captioning model that automatically generates descriptive captions for images using Deep Learning techniques. The architecture is based on the **"Show and Tell"** model, combining Computer Vision and Natural Language Processing.

### Key Features
* **Encoder (Image Processing):** Uses a pre-trained **VGG16** model (Transfer Learning) to extract feature vectors from images.
* **Decoder (Language Modeling):** Uses **LSTM** (Long Short-Term Memory) layers to generate sequence data and handle long-term dependencies.
* **Dataset:** Trained on the **Flickr8k** dataset containing 8,000+ images and 40,000+ captions.

### Model Performance
The model was trained for 20 epochs on a Tesla T4 GPU.
* **Final Loss:** 2.21
* **Optimization:** Adam Optimizer with Categorical Crossentropy loss function.

### Test Results
Below are predictions made by the model on unseen test data:

| Image | 
| :---: | 
| <img width="685" height="380" alt="Ekran Resmi 2025-11-26 20 03 39" src="https://github.com/user-attachments/assets/476b4395-f726-46d2-a666-5096ddcdb1d6" />
 | **"brown dog shaking his head while standing on the sand"**<br>_Demonstrates dynamic action detection._ |
| <img width="658" height="380" alt="Ekran Resmi 2025-11-26 20 02 23" src="https://github.com/user-attachments/assets/dd78fba1-4282-40c8-bada-a0c80299da16" />
| **"group of people are standing on the beach with camels"**<br>_Demonstrates complex scene understanding._ |

---

## Proje Açıklaması
Bu proje, Derin Öğrenme yöntemleri kullanılarak görsellerden otomatik olarak anlamlı İngilizce açıklamalar (altyazılar) üreten bir yapay zeka sistemidir. Proje, Ostim Teknik Üniversitesi Derin Öğrenme dersi kapsamında geliştirilmiştir.

### Temel Özellikler
* **Kodlayıcı (Encoder):** Görüntülerden öznitelik çıkarmak için ImageNet üzerinde eğitilmiş **VGG16** modeli kullanılmıştır.
* **Çözücü (Decoder):** Kelime dizilerini üretmek ve bağlamı korumak için **LSTM** ağları kullanılmıştır.
* **Veri Seti:** 8.000'den fazla görüntü içeren Flickr8k veri seti kullanılmıştır.

### Model Başarımı
Model, Tesla T4 GPU üzerinde 20 Epoch boyunca eğitilmiştir.
* **Eğitim Kaybı (Loss):** 2.21
* **Yöntem:** CNN özellik vektörleri ile LSTM kelime gömüleri (embeddings) birleştirilerek (Merge Architecture) eğitilmiştir.

## 📂 Kurulum ve Kullanım (Installation)

Projeyi çalıştırmak için iki seçeneğiniz var:

### Seçenek 1: Sadece Test Etmek İçin (Önerilen)
Eğitim yapmadan, hazır modeli kullanarak tahmin yapmak için:
1. `Demo_Test.ipynb` dosyasını Google Colab'de açın.
2. Dosyalar arasından `final_model.h5` ve `tokenizer.pkl` dosyalarını indirin ve kodda belirtilen yola koyun.
3. Hücreleri çalıştırıp sonuçları görün.

### Seçenek 2: Modeli Sıfırdan Eğitmek İçin
1. `Training.ipynb` dosyasını açın.
2. Dosyalar arasındaki Flickr8k veri setini indirin.
3. Tüm hücreleri sırasıyla çalıştırın.

---
**Model Dosyaları:**
Modelin boyutu büyük olduğu için GitHub'a yüklenememiştir. `.h5` ve `.pkl` dosyalarını [Buraya Drive Linkini Yapıştır] adresinden indirebilirsiniz.cells to generate captions for new images.

---
**Developer:** Eda VURAL
