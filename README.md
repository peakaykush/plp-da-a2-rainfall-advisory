# Kenya Counties Rainfall Analysis & Planting Advisory (plp-da-a2-rainfall-advisory)

**Student Name:** Peter Kuria  
**Student Email:** peakaykush@gmail.com  
**Cohort:** 1 milliondevs 2026 Data analytics  
**Assignment:** Assignment 2 — NumPy Rainfall Data Cleaning & Advisory  

---

## Project Summary

A farmer-support NGO operating across five Kenyan counties (Nairobi, Nakuru, Kisumu, Mombasa, and Machakos) provides SMS-based agronomic guidance to smallholder farmers on optimal planting windows. This project cleans hand-entered, error-prone monthly rainfall readings from local weather stations, analyzes multi-county rainfall patterns using vectorized NumPy array operations (avoiding manual loops), and computes annual rainfall totals, monthly cross-county averages, peak precipitation months, dry-month counts, and consecutive two-month planting windows. The findings are exported to a standardized `rainfall_summary.csv` file and synthesized into actionable advisories with data-quality caveats.

---

## How to Run

Open and run the analysis notebook directly in Google Colab with all outputs visible:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/peakaykush/plp-da-a2-rainfall-advisory/blob/main/rainfall_analysis.ipynb)

*To run locally:*
```bash
git clone https://github.com/peakaykush/plp-da-a2-rainfall-advisory.git
cd plp-da-a2-rainfall-advisory
pip install -r requirements.txt
jupyter notebook rainfall_analysis.ipynb
```

---

## Planting Advisory

* **Optimal Long Rains Planting (Nairobi, Nakuru, Kisumu, Mombasa):** Smallholders across Nairobi, Nakuru, Kisumu, and Mombasa should prepare their land in March and sow during the **April–May** window, when consecutive two-month rainfall peaks (ranging from 265 mm in Nakuru to 420 mm in Kisumu), ensuring reliable moisture for seed germination and crop establishment.
* **Short Rains Strategy for Machakos:** Unlike the western and coastal counties, Machakos experiences its most reliable rainfall during the short rains, making **November–December** (with a combined 278 mm and a peak of 182 mm in November) the primary planting window; farmers must plant drought-hardy, fast-maturing crops to navigate the county's 6 dry months (< 50 mm).
* **Data Quality Caveat & Localized Verification:** Because Machakos historical records contained missing/invalid entries for April and September that required statistical imputation (imputed at 68 mm), agricultural officers and farmers must treat this advisory as a strategic baseline and verify with real-time Kenya Meteorological Department (KMD) weekly forecasts before committing seeds to the ground.
