# 📚 Semantic Book Recommender with Emotion Aware Search

An AI-powered book recommendation system that uses semantic similarity, emotion classification, and sentiment analysis to suggest personalized book titles based on natural language queries. Built with **LangChain**, **OpenAI embeddings**, and **Gradio**.




---

## 🔍 Features

- 🔗 **Semantic Search**: Uses OpenAI embeddings to find books most similar to a user's input description.
- 💬 **Emotion Classification**: Classifies books by the emotional tone of their descriptions.
- 😊 **Sentiment Analysis**: Evaluates sentiment of descriptions to support mood-based filtering.
- ⚡ **Interactive Gradio UI**: Search, explore, and interact with results in a clean, responsive interface.
- 🧠 **LangChain Integration**: Powered by LangChain for embedding generation and retrieval workflows.

---

## 🧱 Project Structure

```

book-recommender/
│
├── data-exploration.ipynb        # EDA on the book dataset
├── vector-search.ipynb           # Embedding generation + similarity search
├── text-classification.ipynb     # Emotion classification via pre-trained model
├── sentiment\_analysis.ipynb     # Sentiment analysis pipeline
├── gradio-dashboard.py           # Gradio front-end for book recommendations
├── books\_with\_emotions.csv     # Cleaned dataset with labels
└── .env                          # API keys and environment variables (not tracked)

````

---

## 🚀 Demo
## 🖼️ Screenshots

### Main Interface
![Gradio Interface](gradio-interface.png)



Try it locally:
```bash
pip install -r requirements.txt
python gradio-dashboard.py
````

You'll be able to enter a query like:

> *"a heartwarming story about friendship and healing"*
### Search Results
![Search Results](search-results.png)

...and get semantically relevant book recommendations with thumbnails, emotions, and sentiment labels.

### Emotion Classification
![Emotion Filtering](genre-emotion-filtering.png)

![Individual Book View](individual-book-view.png)

---

## 🧠 Techniques Used

| Component              | Approach / Tool                             |
| ---------------------- | ------------------------------------------- |
| Embeddings             | `OpenAI` text embeddings via `LangChain`    |
| Vector Search          | Cosine similarity using FAISS or numpy      |
| Emotion Classification | Pre-trained transformer model               |
| Sentiment Analysis     | `transformers` pipeline (`distilbert-base`) |
| UI                     | `Gradio` interface                          |

---

## 📊 Results

* Embedded **\~2,000 books** with OpenAI's API and saved embeddings locally.
* Supported free-form semantic search with **fast lookup times**.
* Enabled **emotion + sentiment filtering**, improving user satisfaction in qualitative testing.

Screenshots:



---

## 🔒 Environment Variables

You’ll need an `.env` file in your root directory with:

```
OPENAI_API_KEY=your_openai_key_here
```

Do **not** commit your API key.

---

## 💡 Future Improvements

* Add pagination and filters for sentiment/emotion tags.
* Integrate user feedback loop (e.g., thumbs up/down).
* Replace `Gradio` with Streamlit or React frontend for richer UX.
* Fine-tune classification models on book-specific corpora.

---

## 📜 License

This project is licensed under the MIT License.

---
