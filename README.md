🔬 ISIC2018 Cilt Lezyonları Segmentasyonu – PyTorch & U-Net

Bu repo, **Fatih Sultan Mehmet Vakıf Üniversitesi Bilgisayar Mühendisliği Bölümü - Derin Öğrenmeye Giriş (Ödev-2)** kapsamında geliştirilen ISIC2018 veri seti tabanlı cilt lezyonu semantik segmentasyon modelini, eğitim loglarını ve raporunu içermektedir.

---

## 📌 Proje Özeti

- **Amaç:** MedSegBench platformu üzerinden temin edilen ISIC2018 dermoskopi görüntüleri üzerinde cilt lezyonlarını piksel düzeyinde doğru şekilde bölütlemek (semantik segmentasyon).
- **Mimari:** Encoder-Decoder yapılı özelleştirilmiş **U-Net** (Skip-connections, DoubleConv blokları).
- **Kayıp Fonksiyonu:** BCE Loss + Dice Loss bileşimi.
- **Optimizasyon & İzleme:** Adam optimizasyon algoritması (LR: 1e-4), Early Stopping ve TensorBoard log takibi.

---

## 📊 Model Başarımı (Test Sonuçları)

| Metrik             | Değer  |
| ------------------ | ------ |
| **Test Accuracy**  | %86.25 |
| **Test Precision** | %76.95 |
| **Test Recall**    | %72.62 |
| **Test F1-Score**  | %74.72 |
| **Test IoU**       | %59.64 |

---

## 📂 Dizin Yapısı

```text
deeplearning/
├── muhammedeminkorkunc-2021221054.ipynb    # U-Net eğitimi, veri ön işleme ve artırma kodları
├── tensorboard.ipynb                      # TensorBoard metrik görselleştirme notebook'u
├── rapor_2021221054_Protected.pdf         # Detaylı proje analiz raporu
├── LICENSE                                # Telif hakkı ve kullanım koşulları
└── README.md                              # Proje dokümantasyonu
```

👤 Hazırlayan
Muhammed Emin Korkunç (Öğrenci No: 2021221054)

Fatih Sultan Mehmet Vakıf Üniversitesi - Bilgisayar Mühendisliği

GitHub: @muhammedkorkunc

LinkedIn: Muhammed Emin Korkunç

E-posta: muhammedemin.korkunc@gmail.com
