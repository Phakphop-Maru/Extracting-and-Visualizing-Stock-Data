# Extracting and Visualizing Stock Data 📈

## 📌 Project Overview
This project demonstrates the process of **data extraction, processing, and visualization** of stock market data.  
The notebook was developed as part of a data analytics learning path to practice real-world skills in **Python, Pandas, API usage, and Data Visualization**.

The project includes:
- Extracting stock data using **yFinance API** and **web scraping (BeautifulSoup)**  
- Processing & cleaning time-series data with **Pandas**  
- Visualizing stock trends with **interactive Plotly dashboards**  

---

## 🛠️ Tech Stack
- **Programming Language**: Python  
- **Libraries**: Pandas, yFinance, BeautifulSoup, Plotly  
- **Tools**: Jupyter Notebook, Anaconda/Colab  

---

## 📂 Project Structure
```

📦 extracting-visualizing-stock-data
┣ 📜 Extracting and Visualizing Stock Data.ipynb   # Main notebook
┗ 📜 README.md                                     # Project documentation

````

---

## 🔍 Key Steps

1. **Data Extraction**
   - Retrieved stock data using `yfinance` library
   - Performed web scraping with `BeautifulSoup` for additional financial information

2. **Data Processing**
   - Cleaned and organized time-series data with `pandas`
   - Calculated metrics such as average closing prices, trading volumes, and stock trends

3. **Data Visualization**
   - Created interactive visualizations with `plotly`
   - Compared multiple stock performances over time
   - Built candlestick charts and line charts for stock trends

---

## 📊 Example Outputs
### Stock Price Trends
```python
import yfinance as yf
import plotly.graph_objects as go

df = yf.download("AAPL", start="2020-01-01", end="2023-01-01")
fig = go.Figure(data=[go.Candlestick(
    x=df.index,
    open=df['Open'],
    high=df['High'],
    low=df['Low'],
    close=df['Close']
)])
fig.show()
````

*Output:* Interactive candlestick chart of Apple (AAPL) stock prices.

---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/yourusername/extracting-visualizing-stock-data.git
```

2. Install dependencies:

```bash
pip install yfinance beautifulsoup4 pandas plotly
```

3. Open Jupyter Notebook and run:

```bash
jupyter notebook "Extracting and Visualizing Stock Data.ipynb"
```

---

## 📌 Skills Demonstrated

* Data Extraction via **API (yFinance)** and **Web Scraping (BeautifulSoup)**
* Data Wrangling & Cleaning using **Pandas**
* Data Visualization with **Plotly** (interactive dashboards)
* Stock Market Data Analysis

---

## 📈 Connection to Certifications

This project complements skills gained from:

* **Google Data Analytics** – data wrangling, cleaning, visualization
* **IBM Data Analyst** – Python for data science, visualization, SQL integration
* **Tableau BI Analyst** – storytelling and dashboard design (extended to Plotly)
* **Generative AI Data Analyst** – applying data analysis workflows with AI support

---

## 📌 License

This project is for educational purposes only.

---

