# DistilBERT IMDb Sentiment Classification

This project fine‑tunes **DistilBERT** on the **IMDb movie reviews dataset** using the Hugging Face `transformers` and `datasets` libraries.  
It was trained and tested inside **Google Colab using a T4 GPU**.

---

## 🚀 Features
- Loads IMDb dataset (`datasets`)
- Tokenizes using `AutoTokenizer`
- Fine‑tunes DistilBERT for sentiment (positive/negative)
- Uses Hugging Face `Trainer`
- Computes Accuracy + Weighted F1 (via `evaluate`)
- Saves:
  - model
  - tokenizer
  - eval metrics (`eval_metrics.json`)
- Includes inference example

---

## 🧪 Final Model Performance (your run)
- **Accuracy:** ~0.910  
- **Weighted F1:** ~0.910  
- **Eval Loss:** ~0.506  

---

## 📘 How to use this notebook
1. Open the notebook in Google Colab  
2. Go to **Runtime → Change runtime type → GPU (T4)**  
3. Run the notebook cells top‑to‑bottom  
4. Fine‑tuned model will be saved in:  
   ```
   outputs/distilbert-imdb/
   ```

---

## ▶️ Quick Inference Example
```
"POSITIVE"  
"NEGATIVE"
```
(Shown in the notebook’s inference cell.)

---

## 🛠 Run locally (optional)
```bash
pip install -r requirements.txt
python fine_tune_distilbert_imdb.py   # if you add the script
```

---

## 📦 Project Files
- `distilbert_imdb_colab_clean.ipynb` — Clean Colab notebook
- `requirements.txt` — Python dependencies  
- (Optional) `fine_tune_distilbert_imdb.py` — Script version  

---

## 📚 Libraries used
- transformers  
- datasets  
- evaluate  
- accelerate  
- scikit‑learn  
- torch  

---

## 📄 License
For educational use only. DistilBERT weights & IMDb dataset follow their respective licenses.
