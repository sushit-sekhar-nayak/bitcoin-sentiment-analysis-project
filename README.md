# 📈 Bitcoin Market Sentiment vs Trader Performance

This project explores the relationship between **market sentiment** (Fear & Greed Index) and **trader performance** (Closed PnL) using historical trading data. The goal is to uncover patterns that may inform smarter trading strategies.

---

## 🗂️ Project Structure

bitcoin-sentiment-analysis/
├── src/
│ ├──analysis.ipynb
├── data/
│ ├── fear_greed_index.csv
│ └── historical_data.csv
├── outputs/
│ ├── merged_sentiment_trades.csv
├── README.md # This file
└── report.md # Summary of methodology, findings, and challenges

---

## 🛠️ Setup Instructions

### 1. Clone the repository
git clone https://github.com/sushit-sekhar-nayak/bitcoin-sentiment-analysis.git
cd bitcoin-sentiment-analysis

2. Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies
pip install -r requirements.txt

If requirements.txt is not available, manually install:
pip install pandas matplotlib seaborn

Running the Notebook:-
  1. Open Jupyter Notebook:
     jupyter notebook
  2. Run analysis.ipynb step-by-step.
        1. The notebook loads both datasets
        2. Merges them on the date column
        3. Computes average PnL by sentiment classification
        4. Shows visualizations and insights

Sample Output:-
1. Bar chart showing average trader profit by market sentiment
2. Scatter plot of Sentiment Value vs Closed PnL
3. Insights such as: Extreme Greed often leads to better average PnL

Dataset Info:-
Fear & Greed Index:
Source: Alternative.me (manually downloaded)
Columns: date, value, classification
Historical Trader Data:
Provided by Hyperliquid
Columns include: Account, Coin, Size USD, Closed PnL, Timestamp, etc.

External Data Links:-
Since large files are excluded from GitHub, the datasets outputs are stored in a shared Google Drive:
[Google Drive] (https://drive.google.com/drive/folders/155LZvC83w0EJa66SICFnxy_vaz4YfHHS?usp=sharing)

Report:-
See report.md for a detailed explanation of:
1. Methodology
2. Techniques used
3. Challenges and ideas for improvement

Author:-
Sushit Sekhar Nayak
