# 🧮 Project Overview 
1. This project demonstrates the computation and visualization of portfolio Value-at-Risk (VaR) and Expected Shortfall (CVaR) using Python.
2. It estimates potential daily portfolio losses using both Parametric (Variance–Covariance) and Historical methods at 95% and 99% confidence levels.
3. The project also performs simple backtesting to validate VaR predictions and visualize tail risk exposure - essential techniques in Market & Valuation Risk Management.

---

# 🎯 Project Objective
1. Calculate Parametric VaR and Historical VaR for a portfolio of assets.
2. Compute Expected Shortfall (CVaR) to capture tail risk beyond VaR limits.
3. Perform backtesting to evaluate the accuracy of VaR estimates.
4. Visualize return distributions and VaR breaches using Seaborn and Matplotlib.
5. Interpret portfolio risk insights for potential use in Market Risk and FRTB frameworks.

---

# 🧰 Tools & Libraries
1. Python
2. Pandas – data handling and transformation
3. NumPy – numerical computation
4. Matplotlib, Seaborn – visualization
5. SciPy – for statistical functions

---

# 💾 Dataset
1. Historical adjusted closing prices of 5–10 assets (e.g., AAPL, TSLA, JPM, XOM, AMZN) downloaded using the yfinance library.
2. Daily returns calculated to form a multi-asset portfolio (equal-weighted).
3. Period: 2020–2023 (approx. 750 trading days).

---

# 🧩 Methodology
1️⃣ Compute Portfolio Returns
- Combined asset returns into a single equal-weighted portfolio.

2️⃣ Parametric VaR (Variance–Covariance Method)
- Assumes normally distributed returns.
- Uses portfolio mean and standard deviation to calculate VaR.

3️⃣ Historical VaR
- Based purely on observed return percentiles (5th and 1st).

4️⃣ Expected Shortfall (CVaR)
- Calculates average loss beyond the VaR threshold.

5️⃣ Backtesting
- Identifies days when actual portfolio losses exceed VaR estimates.
- Visualized with VaR breaches to validate model reliability.

---

# 📊 Key Results
| Metric             | 95%    | 99%    |
| ------------------ | ------ | ------ |
| Parametric VaR     | -6.56% | -9.69% |
| Historical VaR     | -4.81% | -8.18% |
| Expected Shortfall | -6.70% | -9.41% |

---
# 📈 Visualizations
1️⃣ Distribution of Portfolio Returns with VaR & CVaR (Histogram showing VaR and CVaR cutoffs)

2️⃣ Backtesting VaR Breaches (Line chart showing daily returns vs. VaR thresholds)

---

# 💡 Insights Summary
1. The 99% VaR indicates a potential daily loss of up to 9.7%, while the Expected Shortfall shows that on the worst 1% of days, average losses can reach 9.4%.
2. The Historical VaR is slightly lower than the Parametric VaR, suggesting fewer tail events in the observed data.
3. The backtesting results showed a limited number of VaR breaches, consistent with expected probabilities, indicating a reasonably calibrated VaR model.
4. These findings align with standard practices in Market Risk and FRTB analysis.

---

# 🏁 Conclusion
This project provides a simplified yet realistic framework for quantifying market risk exposure using Python.It demonstrates how key risk metrics like VaR and CVaR are derived, interpreted, and validated.

---

# 🔗 Repository Links
1. 📘 [Notebook – Portfolio_VaR_and_CVaR_Analysis_using_Python.ipynb](https://github.com/PriyasiShah1211/Portfolio-VaR-and-CVaR-Analysis-using-Python/blob/main/Portfolio_VaR_and_CVaR_Analysis_using_Python.ipynb)


