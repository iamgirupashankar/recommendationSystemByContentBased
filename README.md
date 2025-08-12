# recommendationSystemByContentBased
---

# 🎯 Recommendation System using Python & TensorFlow

Recommendation systems are the hidden engine powering platforms like **Netflix, Amazon, Spotify, and YouTube** — personalizing your experience by suggesting what to watch, buy, or listen to next.

In this project, we build a **Content-Based Recommendation System** using a **real Netflix dataset** containing titles, content types, languages, and viewing hours.
By the end, our deep learning model can answer:

> *"If someone liked Wednesday, what else might they enjoy?"* 🍿

---

## 📊 Dataset

We use **Netflix 2023 dataset** with the following fields:

1. **Title**
2. **Available Globally?**
3. **Release Date**
4. **Hours Viewed**
5. **Language Indicator**
6. **Content Type**

💡 *The dataset is perfect for content-based filtering, even without user behavior data.*

---

## ⚙️ Project Workflow

### **Step 1: Load and Understand the Dataset**

* Inspect dataset features.
* Identify key categorical and numerical variables for modeling.

### **Step 2: Data Cleaning & Preprocessing**

* Handle missing values.
* Convert string features to categorical integer encodings.
* Prepare TensorFlow-compatible inputs.

### **Step 3: Build the Neural Recommendation Model**

* Use **Embeddings** to represent categorical variables like content ID, language, and type.
* Embeddings allow the model to learn similarity patterns in the data.

### **Step 4: Model Training**

* Train using **self-supervised learning** — where content metadata predicts similar content.
* The embedding space learns relationships between items.

### **Step 5: Generate Recommendations**

* Compute cosine similarity between embeddings.
* Recommend the closest items in the embedding space.

---

## 🛠️ Tech Stack

* **Python**
* **TensorFlow / Keras**
* **Pandas, NumPy**
* **Scikit-learn**
* **Matplotlib / Seaborn**

---

## 📌 Example Output

If you input:

```
"Wednesday"
```

The model might suggest:

```
"The Addams Family", "Locke & Key", "Stranger Things"
```

based on learned similarities.

---

## 🚀 How to Run

```bash
# 1️⃣ Clone the repo
git clone https://github.com/yourusername/RecommendationSystemByContentBased.git
cd RecommendationSystemByContentBased

# 2️⃣ Install dependencies
pip install -r requirements.txt

# 3️⃣ Run the notebook
jupyter notebook recommendationSystemByContentBased.ipynb
```

---

## 📚 References

* Netflix Dataset (2023)
* TensorFlow Documentation – Embedding Layers
* Content-Based Filtering in Recommender Systems

---

