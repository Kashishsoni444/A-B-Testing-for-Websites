# A-B-Testing-for-Websites
Simulated a full A/B test pipeline in Python to optimize website conversion rates. Covers data generation using binomial distributions, 95% confidence interval calculation, two-proportion z-test hypothesis testing, and real-time sequential monitoring of p-value and lift — visualized with Matplotlib.


# 📊 Website A/B Testing for Conversion Optimization

A Python-based A/B testing simulation notebook that demonstrates how to design, run, analyze, and visualize an A/B test for website conversion rate optimization. Built as part of an internship project at Samatrix.io.

---

## 🧪 What is A/B Testing?

A/B testing (also called split testing) is a method of comparing two versions of something — in this case, two website variants — to determine which one performs better. Visitors are split between Variant A (control) and Variant B (test), and their conversion rates are compared statistically to decide if any observed difference is real or just due to chance.

---

## ✨ What This Notebook Covers

1. **Environment Setup** — Installing and importing all required libraries
2. **Data Simulation** — Generating realistic conversion data for 10,000 visitors per variant
3. **Conversion Rate Analysis** — Computing conversion rates and 95% confidence intervals
4. **Visualization** — Bar charts with error bars showing confidence intervals per variant
5. **Hypothesis Testing** — Two-proportion Z-test to determine statistical significance
6. **Sequential Monitoring** — Live simulation of p-value and lift trajectory over time as visitors accumulate
7. **Results Interpretation** — Clear conclusion on whether Variant B outperforms Variant A

---

## 📈 Key Results

| Metric | Variant A (Control) | Variant B (Test) |
|--------|-------------------|-----------------|
| Visitors | 10,000 | 10,000 |
| True Conversion Rate | 10% | 12% |
| Test | Two-Proportion Z-Test | Significance Level: α = 0.05 |

> If `p-value < 0.05` → Variant B performs significantly better → Reject null hypothesis

---

## 🗂️ Project Structure

```
├── Kashish_Soni_AB_Test_Simulation.ipynb   # Main notebook
└── README.md
```

---

## 🛠️ Tech Stack

| Library       | Purpose                              |
|---------------|--------------------------------------|
| NumPy         | Random data simulation               |
| Pandas        | Data structuring and display         |
| SciPy         | Statistical testing (Z-test)         |
| statsmodels   | Confidence interval calculation      |
| Matplotlib    | Visualization and charts             |

---

## 🚀 Getting Started

### 1. Install dependencies

```bash
pip install numpy pandas scipy statsmodels matplotlib
```

### 2. Open the notebook

```bash
jupyter notebook Kashish_Soni_AB_Test_Simulation.ipynb
```

Or open directly in **Google Colab** or **Kaggle**.

### 3. Run all cells top to bottom

---

## 🧭 Notebook Walkthrough

### Step 1 — Setup
Installs `scipy` and `statsmodels`, imports all libraries, and sets a random seed (`42`) for reproducibility.

### Step 2 — Simulate A/B Test Data
Generates binomial conversion data for two variants:
- Variant A: 10,000 visitors, 10% true conversion rate
- Variant B: 10,000 visitors, 12% true conversion rate

### Step 3 — Compute Conversion Rates & Confidence Intervals
Calculates observed conversion rates and 95% confidence intervals using the normal approximation method.

### Step 4 — Visualize Results
Bar chart comparing both variants with error bars representing the 95% confidence interval.

### Step 5 — Hypothesis Testing
Runs a **Two-Proportion Z-Test** to check whether the difference in conversion rates is statistically significant.

### Step 6 & 7 — Sequential Monitoring
Simulates the test running in real time — batch by batch — and plots how the p-value and lift (B minus A) evolve as more visitors are recorded. This mirrors how real A/B tests are monitored in production.

---

## 📦 Requirements

```
Python >= 3.7
numpy
pandas
scipy
statsmodels
matplotlib
```

---

## 🏫 Project Details

| Field | Details |
|-------|---------|
| Author | Kashish Soni |
| Program | Samatrix.io — BCA AIDA Internship |
| Institution | LNCT University, Bhopal |
| Duration | 4 Weeks |
| Mentor | Vishwas Soni |

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
