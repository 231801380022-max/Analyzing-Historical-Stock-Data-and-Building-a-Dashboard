# Analyzing-Historical-Stock-Data-and-Building-a-Dashboard
Tesla Stock Dashboard (Python, Plotly, Dash)

This project is an interactive dashboard built using Python, Plotly, and Dash to visualize Tesla stock price trends.
Users can explore historical stock data, view line charts, compare metrics, and interact with the dashboard through UI filters.

🚀 Features

📈 Interactive Line Chart of Tesla stock prices

📉 Closing Price, High, Low, and Volume Trends

🔍 Date Range Filters

🧭 Responsive Dashboard Layout

🧮 Data loaded from CSV (Tesla_stock.csv)

🧰 Built using Plotly Graph Objects and Dash Components

📁 Project Structure
Tesla-Stock-Dashboard/
│
├── Tesla_stock.csv          # Dataset (uploaded manually)
├── app.py                   # Dash application file
└── README.md                # Documentation

📦 Installation
1️⃣ Install required libraries

Run this command in your notebook or terminal:

pip install dash plotly pandas


If you are using Google Colab:

pip install dash==2.16.1 jupyter-dash

📂 Add the CSV File

Place Tesla_stock.csv in the same folder as your notebook or Python script.

If using Google Colab, upload it manually:

from google.colab import files
files.upload()

▶️ Running the Dashboard

If running locally (VS Code / Jupyter Terminal):

python app.py


Then open the link shown in the terminal:

http://127.0.0.1:8050/


If using Google Colab, use JupyterDash instead (I can convert it for you if needed).

🛠 Technologies Used

Python 3

Pandas

Plotly

Dash Framework

HTML Components (dash-html-components)

Interactive Graphs (Plotly GO)

📊 Preview of Dashboard Components

Stock Closing Price Line Chart

Range Slider for Date Filtering

Dropdown for Selecting Stock Metrics

Dynamic and Interactive Plot Updates

🧪 Example Code Snippet
fig = go.Figure()
fig.add_trace(go.Scatter(
    x=df.index, 
    y=df['Close'], 
    mode='lines',
    name='Closing Price'
))

🔮 Future Enhancements

📌 Add technical indicators (SMA, EMA, RSI)

⚡ Compare multiple stock datasets (TSLA, AAPL, MSFT…)

💼 Add candlestick chart feature

🗂 Add downloadable reports
