# Graph Machine Learning for Email Classification
# E-posta Sınıflandırması için Graph Machine Learning

 [![Open In Colab]https://colab.research.google.com/drive/1fY36YIeVaZjYUskIOWqFoEbTj92MRur6?usp=sharing

---

## English

This project implements a **graph-based machine learning pipeline** for text/email classification.

Each message is represented as a **node in a graph**, and edges are created between nodes based on **cosine similarity of Bag-of-Words representations**.

Several graph embedding and graph neural network methods are implemented and compared.

### Methods Implemented

- DeepWalk
- Node2Vec
- SiGraC-inspired proximity embeddings
  - HPI (Hub Promoted Index)
  - HDI (Hub Depressed Index)
  - AA (Adamic-Adar)
- Graph Convolutional Network (GCN)

### Pipeline

1. Text dataset loading
2. Dataset sampling
3. Bag-of-Words feature extraction
4. Graph construction using cosine similarity
5. Node embedding generation
6. Node classification
7. Performance comparison

### Results

| Method | Accuracy |
|------|------|
| DeepWalk | 0.575 |
| Node2Vec | 0.605 |
| SiGraC-HPI | 0.680 |
| SiGraC-HDI | 0.665 |
| SiGraC-AA | 0.650 |
| GCN | **0.948** |

### Technologies Used

- Python
- NetworkX
- PyTorch Geometric
- Scikit-learn
- Gensim
- Node2Vec
- Google Colab

---

## Türkçe

Bu proje, metin/e-posta sınıflandırması için **graph tabanlı bir makine öğrenmesi pipeline'ı** uygulamaktadır.

Her mesaj **graf üzerinde bir düğüm (node)** olarak temsil edilir ve düğümler arasında **Bag-of-Words temsillerinin cosine similarity değerine göre kenarlar (edges)** oluşturulur.

Farklı graph embedding yöntemleri ve graph neural network modelleri uygulanarak performansları karşılaştırılmıştır.

### Kullanılan Yöntemler

- DeepWalk
- Node2Vec
- SiGraC esinli yakınlık (proximity) embedding yöntemleri
  - HPI (Hub Promoted Index)
  - HDI (Hub Depressed Index)
  - AA (Adamic-Adar)
- Graph Convolutional Network (GCN)

### Pipeline

1. Metin veri setinin yüklenmesi
2. Veri setinin örneklenmesi
3. Bag-of-Words özellik çıkarımı
4. Cosine similarity kullanarak graph oluşturma
5. Node embedding üretimi
6. Node sınıflandırması
7. Performans karşılaştırması

### Sonuçlar

| Yöntem | Accuracy |
|------|------|
| DeepWalk | 0.575 |
| Node2Vec | 0.605 |
| SiGraC-HPI | 0.680 |
| SiGraC-HDI | 0.665 |
| SiGraC-AA | 0.650 |
| GCN | **0.948** |

### Kullanılan Teknolojiler

- Python
- NetworkX
- PyTorch Geometric
- Scikit-learn
- Gensim
- Node2Vec
- Google Colab
