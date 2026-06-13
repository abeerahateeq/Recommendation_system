[README (1).md](https://github.com/user-attachments/files/28909780/README.1.md)
# 🎯 Recommendation System Using Logic

A smart, interactive recommendation system that matches user preferences to curated content using similarity-based scoring logic.

---

## 📌 Project Overview

This project demonstrates how a simple recommendation engine works — without machine learning. It takes user-selected interests, compares them against a dataset of items, and ranks results by a calculated match score.

Built as a beginner-friendly AI/logic project focusing on **pattern matching**, **data filtering**, and **recommendation concepts**.

---

## 🎯 Goal

Create a simple recommendation system based on user preferences that:
- Takes user input (choices or interests)
- Matches preferences using logic or similarity
- Displays recommended items ranked by relevance

---

## ✨ Features

- **Interest Tag Selection** — Users pick from 12 interest tags (Science, Technology, History, Art, Fiction, etc.)
- **Similarity Scoring** — Each item is scored based on tag overlap with user preferences
- **Match Percentage** — Visual score bar shows how well each item matches
- **Category Filtering** — Filter results by Books, Movies, or Courses
- **Ranked Results** — Top 5 matches displayed in order, with the best match highlighted
- **Real-time Updates** — Results update instantly as preferences change

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, JavaScript |
| Logic | Vanilla JS similarity algorithm |
| Styling | CSS variables, responsive layout |
| Icons | Tabler Icons |

---

## 🧠 How the Recommendation Logic Works

```
Score = (matching tags) / max(user tags, item tags) × 100
```

1. User selects interest tags
2. Each item in the dataset has predefined tags
3. The algorithm finds the intersection of user tags and item tags
4. A match percentage is calculated using the formula above
5. Items are sorted by score (highest first) and top 5 are shown

**Example:**
- User selects: `["Science", "Space", "Adventure"]`
- Item "The Martian" has tags: `["Science", "Adventure", "Technology", "Space"]`
- Matching tags: 3 out of max(3, 4) = 4
- Score: `3 / 4 × 100 = 75%`

---

## 📁 Project Structure

```
recommendation-system/
│
├── index.html          # Main HTML file
├── style.css           # Styling and layout
├── script.js           # Recommendation logic
├── data/
│   └── items.js        # Dataset (books, movies, courses)
└── README.md           # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge)
- No installation or dependencies required

### Run Locally

```bash
# Clone the repository
git clone https://github.com/your-username/recommendation-system.git

# Navigate into the project folder
cd recommendation-system

# Open in browser
open index.html
```

---

## 📊 Dataset

The system includes 12 curated items across 3 categories:

| Category | Examples |
|----------|---------|
| 📚 Books | Sapiens, Thinking Fast and Slow, The Da Vinci Code |
| 🎬 Movies | The Martian, Interstellar, Arrival, Cosmos |
| 🎓 Courses | Deep Learning Fundamentals, UX Design, Data Science |

Each item has 3–4 interest tags used for matching.

---

## 🔑 Key Skills Demonstrated

- **Logic Building** — Writing a scoring algorithm from scratch
- **Pattern Matching** — Comparing user input against structured data
- **Recommendation Concepts** — Understanding similarity and relevance ranking
- **DOM Manipulation** — Dynamic UI updates without a framework
- **Data Handling** — Filtering, sorting, and displaying structured datasets

---

## 🔮 Future Improvements

- [ ] Add user ratings and feedback loop
- [ ] Expand dataset with more items
- [ ] Implement collaborative filtering (user-to-user similarity)
- [ ] Save user preferences to localStorage
- [ ] Add search functionality
- [ ] Connect to a real API (e.g. TMDB for movies, Google Books)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

Built as part of a beginner AI/ML project series focusing on recommendation systems and supervised learning basics.
