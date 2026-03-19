# 🧬 Gaussian Mixture Model (GMM) Implementation from Scratch

Bu proje, Makine Öğrenmesi'nin temel taşlarından biri olan **Gaussian Mixture Model (GMM)** algoritmasının **C** dili kullanılarak, dış bir kütüphane olmaksızın (from scratch) geliştirilmiş halidir.

## 🚀 Proje Genel Bakışı
Bu yazılım, karmaşık veri setlerini istatistiksel olasılıklara dayalı olarak kümelere ayırmak için **Expectation-Maximization (EM)** algoritmasını kullanır. Her bir verinin hangi kümeye ait olduğunu "olasılıksal" olarak hesaplayarak (Soft Clustering), klasik K-Means algoritmasından çok daha esnek sonuçlar üretir.

## 🧠 Teknik Detaylar & Matematiksel Model
- **E-Step (Expectation):** Verilerin mevcut parametrelerle (ortalama, varyans) kümelere ait olma olasılıklarının hesaplanması.
- **M-Step (Maximization):** Hesaplanan olasılıklar üzerinden model parametrelerinin güncellenmesi.
- **Convergence Control:** `EPSILON` eşik değeri ile yakınsama kontrolü yapılarak optimizasyon sağlanır.

## 🛠 Kullanılan Teknolojiler
- **Dil:** C
- **Matematik:** Olasılık Teorisi, Normal Dağılım (Gauss), İstatistiksel Modelleme
- **Yönetim:** Dinamik Bellek Yönetimi (`malloc`/`free`)

## 💻 Nasıl Çalıştırılır?
1. `main.c` dosyasını derleyin: `gcc main.c -o gmm_model -lm`
2. Programı çalıştırın: `./gmm_model`

> **Not:** Derleme sırasında `-lm` bayrağını eklemeyi unutmayın, çünkü `math.h` kütüphanesi kullanılmaktadır.
