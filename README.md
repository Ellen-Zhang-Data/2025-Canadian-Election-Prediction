# 🇨🇦 Predicting the 2025 Canadian Federal Election Outcome

This project uses logistic regression and post-stratification techniques to predict the outcome of the **2025 Canadian Federal Election**, focusing on voter support for the **Conservative Party**, **Liberal Party**, and **NDP**. Our analysis is grounded in the top 5 issues currently influencing Canadian voters: **cost of living, housing, healthcare, economy, and the environment**.

## 📊 Project Overview

Using data from the **2021 Canadian Census** and a survey dataset, this project models the likelihood that individuals with varying demographic characteristics will vote for a specific political party.

We developed three binary logistic regression models — one for each major party — to estimate the probability that an individual would vote for the **Conservatives**, **Liberals**, or **NDP**, given their demographic profile.

### 🔍 Research Motivation

Based on polls and media reports (e.g., Barik, 2023), the Conservative Party is perceived by many Canadians as better equipped to address the top 5 issues. Our hypothesis is that **the Conservative Party is slightly favoured to win** over the Liberal Party in the 2025 election.

---

## 🧠 Methodology

### 1. Data Sources
- 2021 Canadian Census (publicly available)
- Survey dataset containing voter intention
- Supplementary public opinion polls and media reports (Barik, 2023)

### 2. Key Variables
After exploratory data analysis and model selection via **Akaike’s Information Criteria (AIC)**, the following predictors were used:
- `Age`
- `Province`
- `Religion`
- `Education`
- `Income (before tax)`

### 3. Modeling Approach
- Three **binary logistic regression models** were fitted — one for each political party.
- Each model predicts the probability of an individual voting for the respective party.
- Applied **post-stratification** to adjust estimates according to population demographics.

---

## 📈 Results Summary

- **Conservative Party**: ~25.0% predicted vote share (highest)
- **Liberal Party**: ~24.9%
- **NDP**: ~20.0%

Our prediction aligns with current polling and Barik’s (2023) analysis, suggesting a close race between Conservatives and Liberals, with **Conservatives slightly leading**.

---

## 🧩 Limitations

- The 2021 data includes individuals who were **under 18 at the time**, but will be eligible to vote in 2025. Their opinions in 2021 may not reflect their future voting behavior.
- Voter preferences can shift rapidly due to **policy changes** or **external events**.
- Our model is limited to five demographic predictors; other relevant factors (e.g., political affiliation, media influence, campaign effects) are not included.

---

## 🚀 Future Improvements

- Include additional variables (e.g., occupation, urban/rural status, political ideology).
- Incorporate real-time polling and social media sentiment.
- Use ensemble or probabilistic models for higher accuracy.

---

## 📌 Conclusion

This project demonstrates that **logistic regression with post-stratification** can provide meaningful insights into electoral outcomes. While no model can perfectly predict elections due to voter complexity, our estimates closely reflect current research and polling trends.

**Prediction**: The **Conservative Party** is **slightly favoured** to win the 2025 Canadian Federal Election.
