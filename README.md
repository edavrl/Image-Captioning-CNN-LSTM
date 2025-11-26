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

## 📂 Installation and Usage

You have two options to run the project:

### Option 1: For Testing Only (Recommended)
To make predictions using the pre-trained model without training:
1. Open the `Demo_Test.ipynb` file in Google Colab.
2. Download the `final_model.h5` and `tokenizer.pkl` files and place them in the path specified in the code.
3. Run the cells to see the results.

You can download the pre-trained model required to run the project from the link below:
👉 **[Google Drive Link: Model and Files](https://drive.google.com/drive/folders/1DxWbq7R8B_wwqFGjG3nsRmuMUH-0hRRJ?usp=share_link)**

### Option 2: To Train the Model from Scratch
1. Open the `Training.ipynb` file.
2. Download the Flickr8k dataset.
3. Run all cells sequentially.
---

## Proje Açıklaması
Bu proje, Derin Öğrenme tekniklerini kullanarak görseller için otomatik olarak açıklayıcı altyazılar oluşturan bir görsel altyazı modelini uygulamaktadır. Mimarisi, Bilgisayarlı Görüntü İşleme ve Doğal Dil İşleme'yi birleştiren **"Show and Tell"** modeline dayanmaktadır. 

### Temel Özellikler
* **Kodlayıcı (Encoder):** Görüntülerden öznitelik çıkarmak için ImageNet üzerinde eğitilmiş **VGG16** modeli kullanılmıştır.
* **Çözücü (Decoder):** Kelime dizilerini üretmek ve bağlamı korumak için **LSTM** ağları kullanılmıştır.
* **Veri Seti:** 8.000'den fazla görüntü içeren Flickr8k veri seti kullanılmıştır.

### Model Başarımı
Model, Tesla T4 GPU üzerinde 20 Epoch boyunca eğitilmiştir.
* **Eğitim Kaybı (Loss):** 2.21
* **Yöntem:** CNN özellik vektörleri ile LSTM kelime gömüleri (embeddings) birleştirilerek (Merge Architecture) eğitilmiştir.

## 📂 Kurulum ve Kullanım 

Projeyi çalıştırmak için iki seçeneğiniz var:

### Seçenek 1: Sadece Test Etmek İçin (Önerilen)
Eğitim yapmadan, hazır modeli kullanarak tahmin yapmak için:
1. Dosyalar arasından `Demo_Test.ipynb` dosyasını Google Colab'de açın.
2. Dosyalar arasından `final_model.h5` ve `tokenizer.pkl` dosyalarını indirin ve kodda belirtilen yola koyun.
3. Hücreleri çalıştırıp sonuçları görün.

Projeyi çalıştırmak için gerekli olan eğitilmiş modeli aşağıdaki linkten indirebilirsiniz:
👉 **[Google Drive Linki: Model ve Dosyalar](https://drive.google.com/drive/folders/1DxWbq7R8B_wwqFGjG3nsRmuMUH-0hRRJ?usp=share_link)**

### Seçenek 2: Modeli Sıfırdan Eğitmek İçin
1. `Training.ipynb` dosyasını açın.
2. Dosyalar arasındaki Flickr8k veri setini indirin.
3. Tüm hücreleri sırasıyla çalıştırın.

**Developer:** Eda VURAL
