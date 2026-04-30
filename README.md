
# Mohammad Amin Saeini | Machine Learning Engineer 
> **Bridging 7+ years of Mechanical Engineering with Production-Ready AI.**

---

## 🛠 Tech Stack & Knowledge Base

### 🐍 Python Core (High-Level Engineering)
*   **Data Structures**: Expert in list/dict comprehensions, slicing `[::-1]`, and memory management via generators (`yield`).
*   **Production Patterns**:
    ```python
    # Robust error handling & logging (Senior Approach)
    import logging
    def run_inference(features: list) -> float:
        try:
            return model.predict(features)
        except Exception as e:
            logging.error(f"Inference failed at runtime: {e}")
    ```
*   **Process Management**: Multithreading for I/O tasks and Multiprocessing for CPU-bound computations (GIL awareness).

### 📊 Comprehensive ML Model Zoo
**Supervised Learning (Regression & Classification):**
*   **Linear & Logistic Regression**: Baseline modeling and probability estimation.[: 2]
*   **Tree-Based Models**: Decision Trees, Random Forest (Ensemble), XGBoost, and LightGBM. 
*   **Distance & Margin Models**: K-Nearest Neighbors (KNN) and Support Vector Machines (SVM). 

**Unsupervised & Specialized Learning:**
*   **Clustering**: KMeans for pattern discovery and segmentation. 
*   **Anomaly Detection**: Isolation Forest (Crucial for predictive maintenance in industrial systems). 

### 🤖 Machine Learning Lifecycle & Pipeline
*   **Preprocessing**: StandardScaler, LabelEncoder, and OneHotEncoder. 
*   **Evaluation**: Accuracy, Precision/Recall/F1, MSE, and R2 Score. 
*   **Optimization**: Cross-validation and Hyperparameter tuning via `GridSearchCV`. 
*   **Pipeline Pattern**:
    ```python
    from sklearn.pipeline import Pipeline
    # Encapsulating the full workflow for reproducibility
    pipeline = Pipeline([
        ('scaler', StandardScaler()),
        ('model', XGBClassifier(random_state=42))
    ])
    pipeline.fit(X_train, y_train)
    ``` 

### 🐳 Deployment & MLOps
*   **FastAPI**: Building RESTful APIs for model serving with Pydantic for strict input validation. 
*   **Dockerization**:
    *   Building optimized images (`docker build`). 
    *   Managing container lifecycles and Volume mounting for data persistence. 
*   **SQL Mastery**: Complex INNER/LEFT JOINs, Aggregations, and DDL/DML for database management.[cite: 1, 2]
*   **Infrastructure**: Managing AWS resources (S3, IAM) via CLI and version control with Git/GitHub. 

---

## 🚀 The Engineering Edge (Domain Knowledge)
*   **Industrial Expertise**: 7 years in mechanical systems, CNC, and project management.  I understand the physical systems and sensor mechanics behind the data.
*   **Current Focus**: Junior Machine Learning Engineer at Arya Fan Abzar, developing predictive models for sales and market trends. 
*   **Education**: Bachelor in Mechanical Engineering from Zanjan University. 

---

## ✍️ Coding Style & Standards
*   **Consistency**: Strict use of `random_state=42` for experimental reproducibility. 
*   **Clarity**: Preferring snake_case, modular code design, and detailed inline documentation. 
*   **Analysis**: In-depth EDA via `ydata-profiling` before modeling. 

---

## 🌍 Languages
*   **German**: C1 (Professional/Teaching Proficiency) 
*   **English**: B2 (Technical & Business Communication) 
*   **Persian**: Native 

---
