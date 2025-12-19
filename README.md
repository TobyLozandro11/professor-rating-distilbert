# Predicting Professor Review Ratings Using DistilBERT

This project fine-tunes a DistilBERT transformer model to predict 1–5 star professor ratings using written student reviews collected from the PlanetTerp API. The model learns sentiment directly from real student feedback and achieves strong predictive performance.

---

## Project Overview
The goal of this project is to automatically classify the sentiment of professor reviews by predicting the numerical rating (1–5 stars) based solely on the review text.

**Key components:**
- Data collection using the PlanetTerp API  
- Text preprocessing and dataset construction  
- Fine-tuning DistilBERT for sequence classification  
- Evaluation using accuracy, MAE, and confusion matrices  
- Visualization of model performance

---

##  Results
- **Accuracy:** ~73%  
- **Mean Absolute Error:** ~0.50  
- Model performs well at identifying strongly positive and strongly negative reviews  
- Most confusion occurs between neighboring ratings (2↔3, 4↔5)

##  Model Architecture
- Base model: 'distilbert-base-uncased.'
- Fine-tuned classification head (5 labels)
- Optimizer: AdamW  
- Training platform: Google Colab (T4 GPU)

---

##  Example Predictions
| Review Text | True | Predicted |
|------------|------|-----------|
| “Great professor, very helpful and organized.” | 5 | 5 |
| “Lectures were boring and confusing.” | 2 | 2 |
| “Challenging but fair.” | 4 | 3 |

---

## Repository Contents
- `projCode.ipynb` — Full Google Colab notebook  
- `Slide Deck.pdf` — Presentation summarizing the project  

---

## 🛠 Technologies Used
- Python  
- HuggingFace Transformers  
- PyTorch  
- Pandas  
- Matplotlib / Seaborn  
- Google Colab  
- PlanetTerp API  

---

##  Author
**Tobenna Frederick Nwadiaro**  
University of Maryland, College Park
Machine Learning & NLP Project

