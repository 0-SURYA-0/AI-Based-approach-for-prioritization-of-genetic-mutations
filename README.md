# 🧬 AI-Based Approach for Prioritization of Genetic Mutations

Advanced machine learning framework for ranking genetic mutations based on disease relevance using deep learning and biochemical scoring systems.

---

## 🔧 Tech Stack & Requirements

- **Machine Learning**: TensorFlow/Keras (LSTM + k-mer fusion)
- **Bioinformatics**: BLOSUM62 Matrix, Grantham Distance Scoring
- **Data Processing**: NumPy, Pandas, Scikit-learn
- **Visualization**: Matplotlib, Seaborn
- **Analysis**: Jupyter Notebook (`notebooks/main.ipynb`), Python 3.10+

---

## ✨ Features

- 🧬 **Multi-dimensional Mutation Analysis** with sequence and biochemical feature integration
- 🔗 **BLOSUM62 Substitution Matrix** for amino acid change scoring
- 📏 **Grantham Distance Scoring** for physicochemical property analysis
- 🧠 **LSTM Networks** for capturing long-range sequence dependencies
- 🔍 **1D CNN Architecture** for local structural pattern detection
- ⚖️ **Custom Scoring Framework** integrating conservation and structural impact
- 📊 **Advanced Visualizations** highlighting high-impact mutations
- 🎯 **Clinical Relevance Scoring** optimized for precision medicine applications

---

## ⚙️ Setup & Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Vishalspl-0903/AI-Based-Approach-for-Prioritization-of-Genetic-Mutations.git
cd AI-Based-Approach-for-Prioritization-of-Genetic-Mutations
```

### 2️⃣ Environment Setup

Install Python dependencies:

```bash
pip install -r requirements.txt
```

Project structure:

- `scripts/train_model.py` — model training pipeline
- `scripts/preprocess_data.py` — feature extraction utilities
- `scripts/blosum62.py` — BLOSUM62 matrix
- `scripts/grantham_distance.py` — Grantham distance matrix
- `models/` — trained model files (saved here automatically)
- `notebooks/main.ipynb` — main analysis notebook

---

## 📈 Development Roadmap

- [ ] Replace placeholder labels with real pathogenicity annotations
- [ ] Add evaluation metrics notebook (ROC, PR curves) using held-out test set
- [ ] Extend feature set: k-mer frequency normalization, physicochemical embeddings
- [ ] Add unit tests for `scripts/preprocess_data.py` and training pipeline
- [ ] Incorporate additional substitution matrices (PAM, DAYHOFF)

---

## 🤝 Contributing

We welcome contributions! Here’s how to get started:

1. Fork the repository
2. Create a feature branch:  
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. Commit your changes:  
   ```bash
   git commit -m 'Add amazing feature'
   ```
4. Push to the branch:  
   ```bash
   git push origin feature/amazing-feature
   ```
5. Open a Pull Request

### Development Guidelines

- ✅ Follow [PEP 8](https://pep8.org/) style guidelines
- ✅ Include docstrings for new utility functions
- ✅ Add unit tests when expanding preprocessing or model logic
- ✅ Keep `requirements.txt` minimal (remove unused packages before release)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.


