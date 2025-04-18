
# 🧬 AI-Based Approach for Prioritization of Genetic Mutations

![Python](https://img.shields.io/badge/Python-3.8-blue)
![React](https://img.shields.io/badge/React-Frontend-61DAFB?logo=react)
![Flask](https://img.shields.io/badge/Flask-Backend-000000?logo=flask)
![AI](https://img.shields.io/badge/AI-DeepLearning-brightgreen)
![License](https://img.shields.io/badge/License-MIT-purple)

> An AI-powered tool for prioritizing genetic mutations based on their pathogenic potential, enabling efficient identification of risk variants from genomic data.

---

## 📋 Table of Contents

- [📖 Description](#-description)
- [🌟 Features](#-features)
- [🚀 Live Demo](#-live-demo)
- [🧩 Architecture Overview](#-architecture-overview)
- [🛠 Project Setup](#-project-setup)
  - [🔧 Frontend (React)](#-frontend-react)
  - [🧪 Backend (Flask + AI Model)](#-backend-flask--ai-model)
  - [🗄 Database Setup](#-database-setup)
- [🔍 Model Overview](#-model-overview)
- [📊 Sample Output](#-sample-output)
- [🙋‍♂ Authors](#-authors)
- [📃 License](#-license)
- [🌈 Acknowledgments](#-acknowledgments)

---

## 📖 Description

The **AI-Based Approach for Prioritization of Genetic Mutations** project is an advanced tool designed to analyze and prioritize genetic mutations based on their potential clinical impact. By utilizing machine learning techniques, this tool helps geneticists and researchers identify high-risk mutations from large genomic datasets. Additionally, it provides an interactive feature to simulate the mutation's evolutionary impact across different species using data from Ensembl/NCBI.

Built with **React** for the frontend, **Flask** for the backend, and a **PostgreSQL** database to store genomic data and results.

---

## 🌟 Features

- 🔍 **Mutation Prioritization** (*Model 1*): Classify mutations based on pathogenic potential.
- 🧠 **Clinical Impact Prediction** (*Model 2*): Predict whether the mutation is likely to cause disease.
- 🌍 **Mutation Evolution Simulation** (*Novelty Feature*): Simulate how mutations evolved across different species (using Ensembl/NCBI).
- 🎯 Uses **ML Models**: TensorFlow/Keras for mutation prioritization and prediction.
- 🚫 No database required for feature testing, but PostgreSQL integration for storing results and model history.

---

## 🚀 Live Demo

Coming soon...

---

## 🧩 Architecture Overview

mermaid
graph TD
A[User Input Mutation] --> B[Model 1: Mutation Prioritization]
B -->|Low Risk| Z[Return Result]
B -->|High Risk| C[Model 2: Clinical Impact Prediction]
C -->|No Disease| Z
C -->|Likely Disease| D[Model 3: Evolution Simulation]
D --> E[Species Evolution via Ensembl/NCBI]
E --> F[Visualization of Evolutionary Data]

---

## 🛠 Project Setup

### 🔧 Frontend (React)

```bash
# Navigate to frontend folder
cd genomic-mutation-prioritizer/app/frontend

# Install dependencies
npm install

# Start the frontend server
npm start
```

---

### 🧪 Backend (Flask + AI Model)

```bash
# Navigate to backend
cd ../backend

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install required Python libraries
pip install -r requirements.txt
```

**Sample `requirements.txt`:**

```text
Flask
Flask-SQLAlchemy
Flask-Migrate
tensorflow
numpy
pandas
scikit-learn
biopython
```

```bash
# Run Flask server
python app.py
```

---

### 🗄 Database Setup (PostgreSQL)

1. Install **PostgreSQL** on your machine and create a new database.

```bash
psql -U postgres
CREATE DATABASE genomicdb;
```

2. Run migrations to set up the tables.

```bash
flask db upgrade
```

---

## 🔍 Model Overview

| Model | Task | Framework | Input | Output |
|-------|------|-----------|--------|--------|
| *Model 1* | Mutation Prioritization | TensorFlow | Genetic Data (e.g., VCF) | Risk Score (Low/High) |
| *Model 2* | Clinical Impact Prediction | TensorFlow | Mutation Info | Disease Risk (Yes/No) |
| *Model 3* | Evolution Simulation | Custom | Mutation, Species Data | Evolutionary Data (Species Timeline) |

---

## 📊 Sample Output

```json
{
  "Mutation": "KRAS G12D",
  "Model_1": "High Risk",
  "Model_2": "Likely Cancer",
  "Evolution_Simulation": {
    "Conservation": "Conserved in Humans, Mice",
    "Species": ["Human", "Mouse", "Chimpanzee", "Bird"],
    "Impact": "Likely pathogenic due to conservation across species"
  }
}
```

---

## 🙋‍♂ Authors

- **Surya Ha** 🔗 [LinkedIn](https://www.linkedin.com/in/surya-ha-9a0a5a291/)
- **KS Venkatram** 🔗 [LinkedIn](https://www.linkedin.com/in/venkatram-krishnapuram/)
- **Sanggit Saaran KCS** 🔗 [LinkedIn](https://www.linkedin.com/in/sanggit-saaran-k-c-s/)
- **Vishal Seshadri B** 🔗 [LinkedIn](https://www.linkedin.com/in/vishal-seshadri-b-b82074289/)

---

## 📃 License

MIT License – Free for personal & commercial use.

---

## 🌈 Acknowledgments

- **Ensembl** for providing genomic data and evolutionary context.
- **TensorFlow** for powering the machine learning models.
- **Flask** and **React** communities for building the framework.
- **PostgreSQL** for managing genomic data.
- **Bioinformatics** and **AI communities** for making this project possible.

---
