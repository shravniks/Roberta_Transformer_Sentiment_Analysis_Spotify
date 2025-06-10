# 🎧 Spotify Reviews Sentiment Analysis using Transformers

This project explores sentiment analysis on Spotify user reviews using Natural Language Processing (NLP). The primary goal was to compare traditional lexicon-based methods with modern transformer-based approaches.



- **Dataset:** https://www.kaggle.com/datasets/ashishkumarak/spotify-reviews-playstore-daily-update
- **Approach 1 – VADER (Rule-Based):**
  - Used the **VADER** sentiment analyzer from **NLTK**.
  - Quick and interpretable, but limited in handling complex or sarcastic expressions.
- **Approach 2 – RoBERTa (Transformer-Based):**
  - Applied `cardiffnlp/twitter-roberta-base-sentiment` via **Hugging Face Transformers**.
  - Demonstrated improved context understanding and nuanced predictions.
- **Validation:**
  - Used star ratings (1–2: Negative, 3: Neutral, 4–5: Positive) to approximate ground-truth labels for evaluation.
- **Also Tried:**
  - Hugging Face's `pipeline()` for seamless transformer model inference and deployment.

## ⚖️ Key Takeaways

- **VADER** is fast and useful for simple sentiment, but **misses contextual cues and sarcasm**.
- **RoBERTa** performs significantly better on nuanced language but requires **more computational power**.
- **Proxy labels** from review scores helped simulate supervised evaluation in the absence of manual sentiment tags.

