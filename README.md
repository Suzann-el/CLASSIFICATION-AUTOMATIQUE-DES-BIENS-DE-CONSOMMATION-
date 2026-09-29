# 🛍️ Classification d'articles e-commerce — Texte & Image

> Étude de faisabilité d'un moteur de classification automatique d'articles, combinant traitement du langage naturel et vision par ordinateur.

---

## 🎯 Contexte

Dans le cadre du lancement d'une marketplace e-commerce, ce projet explore la faisabilité d'un système capable d'**attribuer automatiquement une catégorie** à un article à partir de sa description textuelle et de son image — pour éviter la saisie manuelle et garantir une classification cohérente.

---

## ⚙️ Ce que fait le projet

Comparaison de plusieurs approches d'extraction de features, texte et image, pour évaluer laquelle offre la meilleure séparabilité des catégories.

### 📝 Features texte

| Approche | Méthode |
|----------|---------|
| Bag-of-words | Comptage simple + TF-IDF |
| Word embedding classique | Word2Vec / FastText |
| Sentence embedding | BERT |
| Sentence embedding | USE (Universal Sentence Encoder) |

### 🖼️ Features image

| Approche | Méthode |
|----------|---------|
| Descripteurs locaux | SIFT / ORB |
| Deep Learning | CNN Transfer Learning |

---

## 📊 Méthodologie

1. **Prétraitement texte** — nettoyage, tokenisation, lemmatisation
2. **Prétraitement image** — redimensionnement, normalisation
3. **Extraction de features** — chaque approche testée indépendamment
4. **Réduction de dimension** — PCA / t-SNE / UMAP pour visualisation
5. **Visualisation** — représentation 2D des clusters pour évaluer la séparabilité

---

## 🛠️ Stack

`Python` `Scikit-learn` `Gensim` `Transformers (BERT)` `TensorFlow` `USE` `OpenCV` `NLTK` `Matplotlib` `t-SNE` `UMAP`

---

## 📁 Structure du projet

```
├── notebooks/
│   ├── 01_preprocessing_texte.ipynb
│   ├── 02_preprocessing_image.ipynb
│   ├── 03_features_texte.ipynb
│   └── 04_features_image.ipynb
└── README.md
```

---

## 📂 Données

Articles e-commerce avec descriptions textuelles et images associées, couvrant plusieurs catégories de produits.
