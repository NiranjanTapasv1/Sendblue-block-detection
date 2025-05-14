# 📬 sendblue-block-detection

A machine learning–based simulation using dummy data modeled after Sendblue’s message schema. This project demonstrates how messaging platforms can detect blocking behavior (such as hitting Apple iMessage rate limits), engineer useful time-based features, and create a flexible ML-ready dataset.

The dummy data was designed to mirror key fields in Sendblue’s actual system, including `sendblueNumber`, message status, error logs, and timestamps.

---

## 🔍 Problem Statements

1. **Detect Apple rate limits** — based on volume/error patterns in short time windows.  
2. **Create ML-friendly datasets** — by aggregating message behavior over time.  
3. **Make predictions flexible** — to support future tasks like conversion or reply prediction.

---

## 🧪 Features of the Notebook

- Simulates message traffic for multiple `sendblueNumber` values  
- Computes rolling 15-minute message and error stats  
- Labels windows as `was_blocked` using threshold logic  
- Trains ML models to predict blocks or simulate conversions  
- Includes visualization for blocked risk and message trends

---

## 📊 Output Visualizations

- Volume vs. Error by block status
  
  <img width="697" alt="image" src="https://github.com/user-attachments/assets/47f134d8-a431-40f5-90b5-1a4c528e3d3a" /></br>
 
- Per-number message/error activity
  <img width="1000" alt="image" src="https://github.com/user-attachments/assets/21224c47-c604-4802-bdf2-31bc7184e515" /></br>


---

## 📁 File Structure

```bash
sendblue-block-detection/
├── Sendblue_code.ipynb                 # Main notebook
├── Simulated_Block_Detection_Data.csv  # Feature data (optional)
├── README.md                           # This file
└── requirements.txt                    # Python dependencies

