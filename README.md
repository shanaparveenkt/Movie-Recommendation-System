# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using **Python, Pandas, and Scikit-learn**.  
The system suggests movies similar to a user’s favorite movie using **TF-IDF Vectorization** and **Cosine Similarity**.

---

## 📦 Libraries Used

| Library | Purpose |
|------|------|
| NumPy | Numerical operations |
| Pandas | Data handling and analysis |
| difflib | Finding closest string matches |
| Scikit-learn | Machine learning tools |
| TF-IDF Vectorizer | Converts text data into numerical vectors |
| Cosine Similarity | Measures similarity between movies |

---

## 📊 Project Workflow

```
Dataset → Data Cleaning → Feature Selection → 
Text Vectorization → Similarity Calculation → 
User Input → Movie Recommendation
```

---

# ⚙️ Step-by-Step Process

---

## 1️⃣ Import Required Libraries

The necessary Python libraries are imported to perform:

- Data manipulation  
- Text processing  
- Similarity calculation  

---

## 2️⃣ Load Dataset

The movie dataset is loaded into a **Pandas DataFrame**.

The dataset contains movie details such as:

| Column | Description |
|------|------|
| Title | Movie name |
| Genres | Movie genre |
| Keywords | Important tags |
| Tagline | Movie description |
| Cast | Actors |
| Director | Movie director |

---

## 3️⃣ Data Exploration

Basic exploration is performed to understand the dataset structure.

Operations performed:

- Display first rows of dataset
- Display last rows
- Check column names
- Check data types
- Statistical summary
- Dataset shape (rows & columns)

```
Rows → Number of movies  
Columns → Number of attributes
```

---

## 4️⃣ Handling Missing Values

Missing values are checked in the dataset.

```
Missing Values → Replaced with Empty Strings
```

This prevents errors during text processing.

---

## 5️⃣ Selecting Important Features

Only the most useful columns are selected for recommendation.

```
Selected Features
│
├── Genres
├── Keywords
├── Tagline
├── Cast
└── Director
```

These features describe the **content of the movie**.

---

## 6️⃣ Combine Text Features

All selected features are merged into a **single text column**.

```
Combined Feature =
Genres + Keywords + Tagline + Cast + Director
```

This creates a **complete description of each movie**.

---

## 7️⃣ Text Vectorization (TF-IDF)

Text data is converted into **numerical vectors** using:

```
TF-IDF Vectorizer
```

TF-IDF gives higher importance to **unique and meaningful words**.

Result:

```
Movie Text → Numerical Feature Matrix
```

---

## 8️⃣ Similarity Calculation

Similarity between movies is calculated using:

```
Cosine Similarity
```

Cosine similarity measures the **angle between vectors**.

| Similarity Score | Meaning |
|------|------|
| 1 | Very similar |
| 0 | No similarity |
| -1 | Opposite |

---

## 9️⃣ User Input

The user enters their **favorite movie name**.

Example:

```
Enter your favourite movie name: Avatar
```

---

## 🔍 10️⃣ Finding Closest Movie Match

Using **difflib**, the system finds the closest movie title.

Example:

```
User Input → Avtar
Closest Match → Avatar
```

This helps handle **spelling mistakes**.

---

## 📈 11️⃣ Finding Similar Movies

Steps performed:

```
Selected Movie
        │
        ▼
Find Movie Index
        │
        ▼
Get Similarity Scores
        │
        ▼
Sort Movies by Similarity
```

Movies with the **highest similarity scores** are selected.

---

## 🎥 12️⃣ Display Recommended Movies

The system prints the **Top 30 similar movies**.

Example output:

```
Movies suggested for you:

1. Guardians of the Galaxy
2. Avengers: Infinity War
3. Thor
4. Captain Marvel
5. Iron Man
...
```

---

# 🧠 Techniques Used

```
Content-Based Filtering
        │
        ├── TF-IDF Vectorization
        ├── Cosine Similarity
        └── String Matching (difflib)
```

---

# 🚀 Key Features

✔ Content-based movie recommendation  
✔ Handles spelling mistakes in movie names  
✔ Uses machine learning similarity techniques  
✔ Beginner-friendly Python implementation  

---

# 📌 Conclusion

This project demonstrates how **Natural Language Processing (NLP)** and **Machine Learning techniques** can be used to build a **Movie Recommendation System**.

The system analyzes **movie content features** and recommends movies that are **most similar to the user's preference**.

---

⭐ Built using **Python, Pandas, and Scikit-learn**
