---

# 📈 Automated Cryptocurrency Analysis with the CoinMarketCap API

This project implements an automated system for querying and analyzing real-time financial data using the CoinMarketCap API. Through a Jupyter Notebook, data is collected every minute for over 5 hours to build a reliable history of multiple cryptocurrencies. The data is then processed, transformed, and visualized using modern analysis and visualization techniques.

---

## 🚀 Technologies Used

- 🐍 Python 3  
- 📦 Libraries: `pandas`, `requests`, `matplotlib`, `seaborn`, `json`, `os`, `time`  
- 📡 CoinMarketCap API  
- 📊 Jupyter Notebook  

---

## ⚙️ Requirements

Before running the notebook, make sure the following dependencies are installed:

```bash
requests==2.31.0  
python-dotenv==1.0.0  
numpy==1.26.0  
pandas==2.1.0  
seaborn==0.12.2  
matplotlib==3.7.2  
jupyter==1.0.0  
ipykernel==6.25.0  
```

---

## 🔐 Setting Up the CoinMarketCap API Key

To protect your access key, this project is set up to read the API Key from an **environment variable**.

### Steps to configure your key:

1. Create a free account at [CoinMarketCap API](https://coinmarketcap.com/api/).  
2. Get your API Key.  
3. Save the key in an environment variable named `CMC_API_KEY`. For example:

**On Linux/macOS:**
```bash
export CMC_API_KEY='your_key_here'
```

**On Windows (CMD):**
```cmd
set CMC_API_KEY=your_key_here
```

**In Jupyter (temporary):**
```python
import os
os.environ['CMC_API_KEY'] = 'your_key_here'
```

---

## ⚙️ Key Technical Features

- 🔁 **Fully automated data consumption**: 333 requests are made at 60-second intervals, collecting over 5 hours of observations.  
- 📥 **Secure API consumption**: Response status (`status_code`) is validated before processing each call.  
- 🧹 **Advanced transformation with pandas**: JSON normalization, field selection, renaming, and column pivoting.  
- 📊 **Multivariable visualization**: Comparison of percentage changes between cryptocurrencies, Bitcoin trend analysis.  
- 💾 **Structured storage** (optional): Data can be saved as CSV or Excel for later analysis.  
- 🛑 **Error handling and robustness**: Exception handling to prevent crashes from invalid responses or network issues.

---

## 📊 Visual Results

### 📈 Bitcoin Price Evolution  
Line chart showing BTC’s price evolution at 1-minute intervals.

![image](https://github.com/user-attachments/assets/97abc027-db81-4fa9-8ea7-79c1bd0e6c5d)

---

### 📊 Percentage Change Comparison  
Comparative visualization between cryptocurrencies (BTC, ETH, ADA, etc.) showing their percentage changes over different time periods.

![image](https://github.com/user-attachments/assets/1fbdb77d-e76b-4009-8227-f985c75fea27)

---

### 🧾 Dataset Preview  
Preview of the normalized DataFrame after collecting data from the API.

![image](https://github.com/user-attachments/assets/83806bea-55f8-4527-b4f4-b44a0d42bf22)

---

## 📂 Project Structure

```
📁 project-root/
├── 📄 Project-ACAPI.ipynb
├── 📄 README.md
├── ⚙️ .env
└── 📄 requirements.txt 
```

---

## 📌 Conclusions

This project allowed me to:

- Master the use of external APIs with authentication.  
- Automate data collection processes at defined time intervals.  
- Work with complex structures like nested JSON responses.  
- Clearly and effectively visualize financial data.  
- Strengthen my data transformation skills using `pandas`.

---

## 👤 Author

**Raul Diaz** — [LinkedIn](https://www.linkedin.com/in/raul-dc/)

---

## 📬 Contact

Got questions, suggestions, or ideas to expand the project?  
Reach out on [GitHub](https://github.com/) or [LinkedIn](https://www.linkedin.com/in/raul-dc/)!

---
