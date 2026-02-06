# 🏥 Système Hybride de Diagnostic Médical par NLP

Ce projet propose une solution intelligente pour classifier **24 pathologies** distinctes à partir de descriptions de symptômes en langage naturel. Il combine la puissance de modèles de langage spécialisés (**BioClinicalBERT**) et une architecture **RAG** (Génération Augmentée par Récupération) pour fournir des réponses explicatives basées sur des cas cliniques réels.

---

## 🚀 Fonctionnalités
- **Classification experte** : Utilisation de BioClinicalBERT fine-tuné sur des données cliniques massives.
- **Moteur RAG** : Recherche de contextes médicaux similaires dans une base de 100 000 interactions médecin-patient (*HealthCareMagic*).
- **Interface Interactive** : Déploiement d'un Chatbot via **Gradio** pour une interaction fluide en temps réel.

---

## 📁 Structure du Projet (Phases)
Le projet est décomposé en 7 notebooks numérotés pour respecter l'ordre logique du pipeline de données :

1. **`1-combining-datasets.ipynb`** : Fusion stratégique des sources de données Hugging Face (*Gretel.ai* et *NeuronZero*).
2. **`2-eda-dataset.ipynb`** : Analyse exploratoire des données (WordClouds, distributions et N-grammes).
3. **`3-preprocessing-code.ipynb`** : Nettoyage par expressions régulières (Regex) et normalisation textuelle.
4. **`4-tf-idf-logistic-regression.ipynb`** : Établissement d'un modèle de référence (Baseline) avec TF-IDF et Régression Logistique.
5. **`5-distilbert-classification.ipynb`** : Première approche par Deep Learning avec un Transformer généraliste léger.
6. **`6-bioclinicalbert-training.ipynb`** : Entraînement et optimisation du modèle expert spécialisé **BioClinicalBERT**.
7. **`7-ChatBot-RAG-Interaction.ipynb`** : Intégration finale de l'architecture RAG et déploiement de l'interface utilisateur.

---

## 🛠️ Installation et Utilisation

### Prérequis
- Python 3.8+
- Un environnement avec GPU (recommandé pour l'exécution des modèles Transformers)

### Installation
1. Clonez le dépôt :
   ```bash
   git clone [https://github.com/HanaeTIZAOUI22/NLP-Diagnostic-Medical.git](https://github.com/HanaeTIZAOUI22/NLP-Diagnostic-Medical.git)
   cd NLP-Diagnostic-Medical
   
