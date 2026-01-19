# Project Zero-Lag: Aadhaar Enrolment Gap Analysis

### 🏆 Hackathon Submission for [Insert Hackathon Name]

## 📌 Project Overview
**Project Zero-Lag** identifies critical "First-Mile Gaps" in India's Aadhaar enrolment ecosystem. By analyzing over 1 million enrolment records, we discovered that specific North-Eastern districts suffer from "Delayed Enrolment Syndrome," where children are not enrolled until school age (5+ years), causing them to miss early childhood welfare benefits.

## 📊 The Metric: "Late Enrolment Index"
We engineered a custom metric to quantify the enrolment delay:
$$\text{Late Enrolment Index} = \frac{\text{School Age Enrolments (5-17)}}{\text{Birth Age Enrolments (0-5)}}$$
* **Index ~ 1.0:** Healthy System (Enrolment happens at birth)
* **Index > 2.0:** Critical Lag (Enrolment happens only at school entry)

## 📂 Repository Structure
* `analysis_script.py`: The main Python script that:
    1. Merges fragmented API datasets.
    2. Cleans state/district nomenclature errors.
    3. Calculates the Lag Index for all districts.
    4. Generates the 4-panel "Zero-Lag Dashboard".
* `Winning_Analysis_4_Charts.png`: The output visualization used in the report.

## 🚀 How to Run
1. Ensure the CSV files (`api_data_aadhar_enrolment_*.csv`) are in the root directory.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
