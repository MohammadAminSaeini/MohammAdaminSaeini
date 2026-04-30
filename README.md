
# Mohammad Amin Saeini | Machine Learning Engineer 
> **Bridging 7+ years of Mechanical Engineering with Production-Ready AI.**[cite: 1]

---

## 🛠 Tech Stack & Knowledge Base

### 🐍 Python Core (High-Level Engineering)
*   **Data Structures**: Expert in list/dict comprehensions, slicing `[::-1]`, and memory management via generators (`yield`).[cite: 2]
*   **Production Patterns**:
    ```python
    # Robust error handling & logging (Senior Approach)
    import logging
    def run_inference(features: list) -> float:
        try:
            return model.predict(features)
        except Exception as e:
            logging.error(f"Inference failed at runtime: {e}")
    ```[cite: 2]
*   **Process Management**: Multithreading for I/O tasks and Multiprocessing for CPU-bound computations (GIL awareness).[cite: 2]

### 📊 Comprehensive ML Model Zoo
**Supervised Learning (Regression & Classification):**
*   **Linear & Logistic Regression**: Baseline modeling and probability estimation.[cite: 2]
*   **Tree-Based Models**: Decision Trees, Random Forest (Ensemble), XGBoost, and LightGBM.[cite: 2]
*   **Distance & Margin Models**: K-Nearest Neighbors (KNN) and Support Vector Machines (SVM).[cite: 2]

**Unsupervised & Specialized Learning:**
*   **Clustering**: KMeans for pattern discovery and segmentation.[cite: 2]
*   **Anomaly Detection**: Isolation Forest (Crucial for predictive maintenance in industrial systems).[cite: 1]

### 🤖 Machine Learning Lifecycle & Pipeline
*   **Preprocessing**: StandardScaler, LabelEncoder, and OneHotEncoder.[cite: 2]
*   **Evaluation**: Accuracy, Precision/Recall/F1, MSE, and R2 Score.[cite: 2]
*   **Optimization**: Cross-validation and Hyperparameter tuning via `GridSearchCV`.[cite: 2]
*   **Pipeline Pattern**:
    ```python
    from sklearn.pipeline import Pipeline
    # Encapsulating the full workflow for reproducibility
    pipeline = Pipeline([
        ('scaler', StandardScaler()),
        ('model', XGBClassifier(random_state=42))
    ])
    pipeline.fit(X_train, y_train)
    ```[cite: 2]

### 🐳 Deployment & MLOps
*   **FastAPI**: Building RESTful APIs for model serving with Pydantic for strict input validation.[cite: 2]
*   **Dockerization**:
    *   Building optimized images (`docker build`).[cite: 2]
    *   Managing container lifecycles and Volume mounting for data persistence.[cite: 2]
*   **SQL Mastery**: Complex INNER/LEFT JOINs, Aggregations, and DDL/DML for database management.[cite: 1, 2]
*   **Infrastructure**: Managing AWS resources (S3, IAM) via CLI and version control with Git/GitHub.[cite: 2]

---

## 🚀 The Engineering Edge (Domain Knowledge)
*   **Industrial Expertise**: 7 years in mechanical systems, CNC, and project management.[cite: 1] I understand the physical systems and sensor mechanics behind the data.
*   **Current Focus**: Junior Machine Learning Engineer at Arya Fan Abzar, developing predictive models for sales and market trends.[cite: 1]
*   **Education**: Bachelor in Mechanical Engineering from Zanjan University.[cite: 1]

---

## ✍️ Coding Style & Standards
*   **Consistency**: Strict use of `random_state=42` for experimental reproducibility.[cite: 2]
*   **Clarity**: Preferring snake_case, modular code design, and detailed inline documentation.[cite: 2]
*   **Analysis**: In-depth EDA via `ydata-profiling` before modeling.[cite: 2]

---

## 🌍 Languages
*   **German**: C1 (Professional/Teaching Proficiency)[cite: 1]
*   **English**: B2 (Technical & Business Communication)[cite: 1]
*   **Persian**: Native[cite: 1]

---
