# 🏋️ Fitness Tracker using Machine Learning

A complete end-to-end machine learning project for classifying barbell exercises and counting repetitions using wearable sensor data (accelerometer + gyroscope).

## Team project & my contribution

This is Ahmed Hossam's portfolio fork of a project developed collaboratively with the team. The original authorship, commit history, and contributor credits are preserved.

**My recorded contributions:**

- **Sensor-data visualization:** Matplotlib plots comparing sensor axes, participants, and exercise categories — [`e53c85e`](https://github.com/AhmedxHossam/FitnessTracker/commit/e53c85e4cbb2f32014ef9008b8d7a30e2042d02e).
- **Exercise comparisons:** updates to the visualization script and an accelerometer comparison figure — [`3ec4927`](https://github.com/AhmedxHossam/FitnessTracker/commit/3ec49278454cb615131a0b3e6d1a883d9160e9ff).
- **Model-training workflow:** updates to the training script, learning-algorithm utilities, and an exploration notebook — [`372158c`](https://github.com/AhmedxHossam/FitnessTracker/commit/372158ce5b5523d81b4bf1ee8a7aa4f8c975d19a).

[Original team repository](https://github.com/M0hamed-Eid/FitnessTracker) · [Final report](reports/ML_Fitness_Tracker_Project.pdf) · [Presentation](reports/ML_Fitness_Tracker_Project.pptx)

---


## 📌 Project Overview

This project builds a full ML pipeline that transforms raw sensor data into meaningful fitness insights:

- 🏷️ Exercise Classification (Bench Press, Squat, Row, etc.)
- 🔁 Repetition Counting using signal processing
- 📊 Performance analysis across multiple users

---

## ⚙️ Machine Learning Pipeline

1. Data Collection (Wearable Sensors)
2. Data Cleaning & Preprocessing
3. Exploratory Data Analysis (EDA)
4. Outlier Detection
5. Feature Engineering
6. Model Training & Evaluation
7. Repetition Counting Algorithm

---

## 🤖 Models Implemented

- Naive Bayes
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest ⭐ (Best Performance)
- Neural Network

---

## 📊 Results

- ✅ ~99% Accuracy using Random Forest
- ✅ Strong generalization across users
- ✅ Reliable repetition counting

These are the original team's reported results. See the [final report](reports/ML_Fitness_Tracker_Project.pdf) for the experiment details; the models were not retrained for this portfolio documentation update.

---

## 📂 Project Structure
```text
data/              # Raw, interim, and processed datasets
docs/              # Project documentation
models/            # Trained models and predictions
notebooks/         # Analysis and experimentation notebooks
references/        # Data dictionaries and manuals
reports/           # Generated analysis and reports
├── ML_Fitness_Tracker_Project.pdf
├── ML_Fitness_Tracker_Project.pptx
└── figures/        # Pipeline, signal plots, and model-evaluation figures
src/               # Core ML pipeline (data, features, models, visualization)
environment.yml    # Conda environment configuration
README.md          # Project overview
requirements.txt   # Python package dependencies
```

---

## 🧠 Project Pipeline

![Pipeline](reports/figures/pipeline.png)

---

## 📊 Sample Results

![Confusion Matrix](reports/figures/figures/confusion_matrix.png)

---

## 📎 Documentation

- 📄 [Final Report](reports/ML_Fitness_Tracker_Project.pdf)
- 🎤 [Presentation](reports/ML_Fitness_Tracker_Project.pptx)

---

## 🚀 How to Run

The original project environment is defined in [`environment.yml`](environment.yml), which specifies Python 3.8.15 and the original NumPy, pandas, and Matplotlib versions. The current `requirements.txt` is empty and does not install the application's dependencies.

From the repository root, use Conda to create the original environment, then install the additional libraries imported by the source:

```bash
conda env create -f environment.yml
conda activate tracking-barbell-exercises
python -m pip install scikit-learn scipy seaborn
```

The scripts resolve dataset paths relative to their working directory. Run each example from its own source folder:

```bash
# From the repository root: inspect the sensor visualizations
cd src/visualization
python visualize.py
cd ../..

# Train/evaluate using the bundled engineered features
cd src/models
python train_model.py
cd ../..
```

The visualization example reads `data/interim/01_data_processed.pkl`; training reads `data/interim/03_data_features.pkl`. Both are present in the repository. The complete source also includes preprocessing, feature-engineering, and repetition-counting scripts under `src/`.

These instructions are based on the environment manifest and source imports. A fresh environment installation and model-training run were not performed for this documentation update; the additional packages above are not pinned in the original manifest.

---

## 👨‍💻 Contributors

- **Mohammed Eid** — [GitHub Profile](https://github.com/M0hamed-Eid)
- **Ahmed Hossam** — [GitHub Profile](https://github.com/AhmedxHossam)
- **Mohammed Salah** — [GitHub Profile](https://github.com/msalah65654-hue)

---


## 🔗 Repository
👉 [https://github.com/M0hamed-Eid/FitnessTracker](https://github.com/M0hamed-Eid/FitnessTracker)
