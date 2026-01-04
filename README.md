# 🥦 Food Macros Search Engine

A fast, Python-based **CLI search engine** that lets users type food names and instantly retrieve **macronutrient information** from a pre-processed USDA Foundation Foods dataset.

Search suggestions are generated using a **trie (prefix tree)**, and results are efficiently linked to nutrient data using an **inverted index** — all running inside a Python terminal environment.

---

## 🚀 Features

- 🔍 **Autocomplete food search** using a trie (prefix tree) for real-time suggestions.
- 📌 **Inverted index lookup** to map words → food IDs → macro values.
- 📘 Outputs **macronutrient data** (e.g., calories, protein, carbs, fats) from USDA macros CSV.
- 🧠 Designed for speed and simplicity inside a terminal.
- 🧪 Includes a data preprocessing Jupyter Notebook demonstrating how to generate the search engine CSVs from raw USDA data.
- 📦 Pre-processed CSVs (`raw_foods_words.csv`, `food_dictionary.csv`, and `food_macros.csv`) included so you can run the engine immediately.

---

## 🧠 Motivation

Finding **accurate nutrition data** quickly can be tedious. Instead of browsing large CSVs or slow search scripts, this project delivers fast responses with algorithmic search structures like tries and inverted indexes — techniques used in real-world search engines. This project showcases:

✔️ Efficient data structures (Trie, inverted index)  
✔️ Practical CSV preprocessing & linking  
✔️ Python scripting and Jupyter data workflows  

---

## ⚙️ How It Works

1. **Trie autocompletion**  
   The search engine uses a trie built from all words in the food dataset so that as you type, it suggests valid completions.

2. **Matching food terms**  
   Matches are linked via an **inverted index** (`food_dictionary.csv`), mapping search tokens to food IDs.

3. **Results retrieval**  
   Using those IDs, macro data is pulled from `food_macros.csv` and displayed to the user.

---

## 📁 Files & Structure

| File | Purpose |
|------|---------|
| `search_engine.py` | Main CLI search script |
| `raw_foods_words.csv` | Word list used to build the trie |
| `food_dictionary.csv` | Inverted index: words → food IDs |
| `food_macros.csv` | Nutrient data (macros) indexed by food ID |
| `*.ipynb` | Data preprocessing notebooks |
| `.gitignore` | Ignore configs and outputs |

---

## 💡 Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Seth-Wr/Food-Macros-Search-Engine.git
   cd Food-Macros-Search-Engine
   cd USDA_Search_Engine
2. **Download Dependencies**
   ```bash
   pip install pandas
3. **Start Engine**
   ```bash
   python Search_Engine.py 

