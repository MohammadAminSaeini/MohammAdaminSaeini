## Hi 

---
name: ml-knowledge-base
description: >
  Personal ML/Data Science knowledge base for Mohammad Amin Saeini. Use this skill
  whenever the user asks how to do something in Python, pandas, numpy, scikit-learn,
  SQL, Git, Docker, AWS, or any ML workflow step. Also trigger when the user asks to
  explain a concept they've studied, debug their code, extend a pattern from their
  notebook, write code in their personal style, or review/improve existing code.
  This skill knows the user's exact coding patterns and preferred approaches — always
  check here before answering generic ML/DS questions.
---
 
# Mohammad Amin's ML Knowledge Base
 
This skill captures the user's personal study notes, preferred code patterns, and
known techniques from their Machine Learning notebook. When answering questions,
prefer the patterns and libraries the user already knows. Fill gaps with best
practices, but stay close to their established style.
 
---
 
## What the user knows — topic map
 
### Python Core
- **Arithmetic**: `**` power, `//` floor division, `%` modulo, `f"{x:.2f}"` formatting
- **Strings**: f-strings, slicing `[::-1]`, `.replace()`, `.split()`, `.strip()`
- **Data structures**: list (append/extend/insert/remove/map/filter), tuple (immutable, usable as dict key), dict (`{key: value}`), set
- **Control flow**: for/while loops, list comprehensions, `enumerate()`, `zip()`
- **Functions**: `*args`, `**kwargs`, lambda, generators (`yield`)
- **OOP**: classes, `__init__`, inheritance
- **File I/O**: `open()`, context managers (`with`)
- **Multithreading vs Multiprocessing**: threads = I/O-bound, processes = CPU-bound, GIL awareness
- **Memory management**: use functions to scope heavy computations; garbage collection awareness
- **Virtual environments**: `python3 -m venv .venv`, activate, `pip freeze > requirements.txt`
### Git / GitHub
```bash
git init / git clone <url>
git pull / git status / git add . / git reset
git commit -m "message"
git push -u origin main
git push -uf origin main        # force overwrite remote
git branch / git switch -c new-branch
git branch -D branch-name
```
 
### SQL
- SELECT, WHERE, ORDER BY, LIMIT/OFFSET
- Aggregates: COUNT, SUM, AVG, MIN, MAX, GROUP BY, HAVING
- JOINs: INNER, LEFT, RIGHT, FULL OUTER, CROSS
- Set ops: UNION / UNION ALL, INTERSECT, EXCEPT
- DML: INSERT, UPDATE, DELETE, TRUNCATE
- DDL: CREATE TABLE, DROP TABLE, ALTER TABLE
### Pandas / Data Analysis
```python
import pandas as pd
df = pd.read_csv('file.csv')
df.head() / df.info() / df.describe()
df['col'].unique() / df['col'].nunique() / df['col'].value_counts()
df[df['col'] > value]           # filtering
df.groupby('col').agg({'col2': 'mean'})
df.drop(columns=['col'])
df.fillna(value) / df.dropna()
df.isnull().sum()
```
- Profiling tools known: `ydata-profiling` (ProfileReport), `sweetviz`
- Note: Mito (visual editor) only works in JupyterLab, NOT VS Code
### NumPy
```python
import numpy as np
np.array([]) / np.zeros() / np.ones() / np.arange() / np.linspace()
arr.reshape() / arr.T  # transpose
np.mean() / np.std() / np.median()
np.dot() / np.linalg.norm()
```
 
### Matplotlib / Visualization
```python
import matplotlib.pyplot as plt
plt.plot() / plt.scatter() / plt.hist() / plt.bar()
plt.xlabel() / plt.ylabel() / plt.title() / plt.legend()
plt.show() / plt.savefig()
```
 
### Scikit-learn (ML pipeline)
```python
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler, LabelEncoder, OneHotEncoder
from sklearn.pipeline import Pipeline
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
                            mean_squared_error, r2_score
 
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)  # IMPORTANT: only transform, never fit on test set
 
model.fit(X_train_scaled, y_train)
y_pred = model.predict(X_test_scaled)
```
 
**Models the user has studied:**
- Linear Regression, Logistic Regression
- Decision Tree, Random Forest
- KNN
- SVM
- Gradient Boosting (XGBoost / LightGBM patterns likely known)
- Clustering: KMeans
**Key concepts:**
- Train/test split, cross-validation
- Overfitting vs underfitting
- Feature engineering, feature importance
- Hyperparameter tuning (GridSearchCV)
- Confusion matrix, precision/recall/F1
### Docker
```bash
# Images
docker pull <image>
docker build -t my_image .
docker images / docker rmi my_image
 
# Containers
docker run -d --name my_container -p 8080:80 my_image
docker run -v /host/path:/container/path my_image   # volume mount
docker start/stop/restart my_container
docker rm my_container
docker container prune -f
 
# Interaction
docker ps / docker ps -a
docker exec -it my_container bash
docker logs -f my_container
docker cp my_container:/container/path /host/path
docker stats my_container
 
# Dockerfile keywords known: FROM, RUN, COPY, WORKDIR, EXPOSE, CMD, ENV
```
 
### FastAPI
```python
from fastapi import FastAPI
app = FastAPI()
 
@app.get("/")
def read_root():
    return {"message": "Hello"}
 
@app.post("/predict")
def predict(data: InputModel):
    result = model.predict(data.features)
    return {"prediction": result}
```
- Run with: `uvicorn main:app --reload`
- Pydantic for input validation
### AWS (basics)
- **IAM**: users, groups, roles, policies (Allow/Deny), inline vs managed policies
- **Access keys**: for programmatic access via CLI (`aws configure`)
- **S3**: bucket operations (known patterns)
- **Billing**: Free tier monitoring, budget alerts
- **Cloud Shell**: browser-based terminal
---
 
## User's coding style preferences
 
- Uses Jupyter notebooks for exploration
- Prefers f-strings for formatting
- Adds comments with `#` inline, not docstrings
- Uses snake_case for variables
- Keeps imports at top of cell
- Likes to inspect data with `.head()`, `.info()`, `.describe()` before modeling
- Uses `random_state=42` consistently for reproducibility
---
 
## How to use this skill
 
**When user asks a how-to question:**
Check if the topic is covered above → use the exact pattern they know → extend it for their specific need.
 
**When user shares broken code:**
Match their style, fix the issue, explain briefly why it broke.
 
**When user asks to explain a concept:**
They're an ML engineer with C1 German, strong project management background, and are building hands-on ML skills. Explain with concrete examples, not just theory. Relate to their known patterns where possible.
 
**When user asks about something NOT in this notebook:**
Answer normally but note that adding it to the notebook would be a good idea for their reference.
