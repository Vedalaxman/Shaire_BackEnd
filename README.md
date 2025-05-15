# Shaire_BackEnd
A Smart Bill Extraction and Expense Management App

## Deployment
🚧 **Currently under development**  
(Deployment link will be added once the app is live)
🔗 [Check for updates here](https://github.com/rishitdutta/shaire)

---

## Overview
Shaire is an AI-powered expense management app that simplifies how users track, predict, and manage their spending. It extracts relevant data from receipts, predicts future expenses, and categorizes transactions using machine learning techniques.

---

## ML Features

### 📤 Bill Extraction
- Extracts item names, prices, quantities, and totals from scanned bills.
- OCR-based input parsing followed by custom ML post-processing.

### 📊 Expense Prediction
- Predicts future expenses based on historical data.
- Models used:
  - **Linear models** for small/medium data.
  - **LSTM** for larger datasets with time-series characteristics.

### 🗂️ Category Prediction
- Automatically classifies expenses into categories (e.g., Food, Travel, Bills).
- Uses:
  - **TF-IDF** vectorization
  - **Nearest Neighbor Similarity**
  - Lightweight neural networks for improved classification

---

## Dataset
- Collected from real-world bills and manual entries.
- Fields include:
  - `Date`, `Time`, `Money`, `Category`, `Items`, etc.
- Data is preprocessed, cleaned, and used for both supervised and sequence learning tasks.

---

## Backend & Infrastructure

- **Supabase** for:
  - Authentication
  - Real-time database
  - API services

- **ML Models** are trained offline using Python libraries and exported using:
  - `joblib` or `pickle`

---

## Workflow

1. 📷 Upload/scan a bill.
2. 🧠 Extract relevant fields using OCR + ML.
3. 📈 Predict upcoming expenses based on past trends.
4. 🗃️ Categorize transactions intelligently.
5. 📊 Visualize and manage your expenses via dashboard (coming soon).

---

## File Structure (Coming Soon)

- `app/` — frontend and API integrations
- `ml_models/` — model weights:  
  - `bill_extractor.pkl`  
  - `expense_predictor.pkl`  
  - `category_classifier.pkl`
- `data/` — sample training and test datasets

---

## Author
Peddi Veda Laxman

---

## Coming Soon
- Web dashboard for visualization
- Budget alerts and summaries
- Multi-user bill splitting
- Full Android app deployment (.apk will be linked in future)

