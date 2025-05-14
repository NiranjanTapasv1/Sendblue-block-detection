# 📬 sendblue-block-detection

A machine learning–based simulation to identify potential Apple iMessage rate limits and blocked senders. This project uses synthetic message data to show how Sendblue-like platforms can detect blocking behavior, engineer time-based features, and build reusable ML pipelines.

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
- Per-number message/error activity  
- Block-rate heatmap

---

## 📁 File Structure

```bash
sendblue-block-detection/
├── Sendblue_code.ipynb                 # Main notebook
├── Simulated_Block_Detection_Data.csv  # Feature data (optional)
├── README.md                           # This file
└── requirements.txt                    # Python dependencies

