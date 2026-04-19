# 📊 Quant Risk Modeling: VaR & Expected Shortfall

## 🚀 Overview
This project implements advanced risk modeling techniques to measure and evaluate market risk using **Value at Risk (VaR)** and **Expected Shortfall (ES)**.

It uses **real historical stock data (AAPL)** to compute risk metrics and validate models through statistical backtesting.

---

## 🧠 Models Implemented

### 📉 Value at Risk (VaR)
- Historical Simulation  
- Variance-Covariance (Parametric)  
- Monte Carlo Simulation  

### 📊 Expected Shortfall (ES)
- Historical ES  
- Parametric ES  
- Monte Carlo ES  

---

## ⚙️ Methodology

### 1. Data Processing
- Loaded historical price data  
- Computed daily returns using percentage change  

### 2. Risk Estimation
- Calculated VaR at 95% confidence using three methods  
- Computed Expected Shortfall to capture tail risk  

### 3. Backtesting
- **Kupiec Test** to validate model accuracy  
- **Traffic Light Test** to classify model performance  

---

## 📊 Key Results

### VaR (95%)
- Historical VaR: **-2.99%**  
- Monte Carlo VaR: **-3.20%**  
- Parametric VaR: **Not reliable (inconsistent results)**  

### Expected Shortfall (95%)
- Historical ES: **-4.35%**  
- Monte Carlo ES: **-4.03%**  
- Parametric ES: **Unstable**  

---

## 🔍 Insights
- Historical and Monte Carlo methods produced **consistent and realistic risk estimates**  
- Parametric model showed **poor reliability under real market conditions**  
- Expected Shortfall captures **tail risk better than VaR**  

---

## 🧪 Backtesting Results
- Historical model passed Kupiec Test and remained in **Green Zone**  
- Monte Carlo model showed acceptable accuracy  
- Parametric model failed under exception analysis  

---

## ⚠️ Key Takeaways
- VaR alone is insufficient → ES provides deeper risk insight  
- Model validation is critical before real-world application  
- Real data exposes weaknesses in simplified assumptions  

---

## 🔧 Future Improvements
- Use multi-asset portfolios instead of single stock  
- Incorporate volatility clustering (GARCH models)  
- Improve Monte Carlo realism with fat-tailed distributions  
