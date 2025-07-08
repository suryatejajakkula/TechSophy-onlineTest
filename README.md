## Medication Interaction Checker

This project helps **check for drug–drug interactions (DDIs)** and alerts healthcare professionals with severity, recommendations, and safer alternatives.  
It uses the **DDInter dataset**, manually added interactions, and a basic **ML model** to predict severity.


## 📋 Features

- ✅ Detects known drug–drug interactions from DDInter data.
- ✅ Adds common clinical interactions manually.
- ✅ Predicts severity using Random Forest (if enough data is available).
- ✅ Adjusts severity based on patient age & conditions.
- ✅ Suggests alternative drugs when possible.
- ✅ Generates clear alerts with confidence scores.


## Steps
### Step 1: Prepare the dataset

Place your **DDInter dataset** file:
ddinter_downloads_code_V.csv


inside your Google Drive at:
/My Drive/ddinter_downloads_code_V.csv


### Step 2: Run the script

In Google Colab or locally, run:
```bash
python medication_interaction_checker.py
It will:

Mount Google Drive

Load the dataset

Print alerts in JSON format

📊 Example Alert
{
  "severity": "MAJOR",
  "drugs": ["warfarin", "aspirin"],
  "description": "Potential for increased bleeding risk.",
  "recommendation": "Monitor for signs of bleeding.",
  "confidence": "92.00%",
  "alternative": "Consider apixaban or clopidogrel"
}
📁 Files
medication_interaction_checker.py — main Python script.

ddinter_downloads_code_V.csv — DDInter dataset (required).


📖 Data Source
DDInter — Drug–Drug Interaction database.

