<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>S&P 500 Daily Prediction Project</title>
</head>
<body style="font-family: sans-serif; line-height: 1.6; max-width: 800px; margin: auto; padding: 20px;">

  <h1>📈 S&P 500 Daily Movement Prediction using Machine Learning</h1>

  <p>This Jupyter notebook predicts whether the <strong>S&P 500 index</strong> will go up or down the next day using historical data and a binary classification approach. It uses basic machine learning techniques to model stock trends.</p>

  <h2>💡 Objective</h2>
  <p>To forecast the next day's price movement of the S&P 500 Index using historical trading data.</p>

  <h2>⚙️ Tech Stack</h2>
  <ul>
    <li>Python 3.10+</li>
    <li>Jupyter Notebook</li>
    <li>Pandas</li>
    <li>Numpy</li>
    <li>Matplotlib</li>
    <li>scikit-learn</li>
    <li>yfinance</li>
  </ul>

  <h2>📥 Dataset</h2>
  <p>Data is pulled using the Yahoo Finance API via the <code>yfinance</code> Python package.</p>
  <p><strong>Ticker:</strong> ^GSPC (S&P 500 Index)</p>

  <h2>🚀 How to Run</h2>
  <p>Make sure you have Python and Jupyter Notebook installed. Then follow these steps:</p>

  <pre><code># 1. Create and activate a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 2. Install required packages
pip install pandas numpy matplotlib scikit-learn yfinance notebook

# 3. Launch Jupyter Notebook
jupyter notebook

# 4. Open the notebook file (e.g., sp500_prediction.ipynb) and run cells one by one
</code></pre>

  <h2>⚠️ Having Trouble with yfinance?</h2>
  <p>If <code>yfinance</code> fails to fetch data (due to connection or update issues), here are two alternatives:</p>

  <ol>
    <li>
      Use <a href="https://www.kaggle.com/datasets/camnugent/sandp500" target="_blank">this Kaggle S&P 500 dataset</a>.
      <ul>
        <li>Download the CSV</li>
        <li>Replace the yfinance data import code with <code>pd.read_csv("your_file.csv")</code></li>
      </ul>
    </li>
    <li>
      Try <a href="https://pypi.org/project/yahoo-finance-interface/" target="_blank">Yahoo Finance Interface</a> as a backup API.
    </li>
  </ol>

  <h2>📊 Features Used</h2>
  <ul>
    <li>Open, High, Low, Close, Volume</li>
    <li>Tomorrow’s close price (shifted)</li>
    <li>Target (1 if Tomorrow > Today’s Close, else 0)</li>
  </ul>

  <h2>❤️ Author</h2>
  <p>Made with curiosity by <strong>Swetha</strong>, a passionate AI graduate exploring financial data with ML.</p>
  <p>If you found this interesting or want to collaborate, feel free to connect!</p>

</body>
</html>
