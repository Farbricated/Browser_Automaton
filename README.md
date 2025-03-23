# 🤖 Browser Automaton 🌐

This repository contains the Jupyter Notebook `Browser_Automaton.ipynb`, which automates web interactions using Python.

## 📜 Description
The notebook leverages APIs and web scraping techniques to automate browser-based tasks such as searching the web and extracting useful information.

## 🛠️ Tools & Libraries Used
- 🔎 **SerpAPI** - For fetching search results
- 🏗 **BeautifulSoup** - For web scraping and parsing HTML
- 🌐 **Requests** - For making HTTP requests
- 🤖 **Google Generative AI** - For advanced text processing
- 🎨 **Gradio** - For creating an interactive web UI

## 📝 Sample Code
```python
from serpapi import GoogleSearch

SERPAPI_KEY = "your_serpapi_key"

def google_search(query):
    params = {"q": query, "api_key": SERPAPI_KEY, "num": 5}
    search = GoogleSearch(params)
    return search.get_dict().get("organic_results", [])

# Example Usage
results = google_search("Automated Web Scraping")
print(results[:3])  # Display first 3 search results
```

## 📜 License
This project is licensed under the MIT License. 📄
