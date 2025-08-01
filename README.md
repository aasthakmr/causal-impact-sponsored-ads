# Causal Impact of Sponsored Search Ads  

## 📌 Overview  
This project evaluates the true impact of sponsored search ads on branded keyword traffic and ROI for Bazaar.com. Using a natural experiment where Google ads were paused for three weeks, the analysis applies **Difference-in-Differences (DiD)** to measure incremental traffic lift and calculate realistic ROI, correcting for overestimation from naive attribution methods.  

---

## 🔑 Key Insights  
- **Naive ROI is inflated:** Treating all ad clicks as incremental ignores users who would have visited organically.  
- **Measured impact:** Google traffic dropped by **~67%** during the ad pause, isolating the causal effect of paid ads.  
- **ROI from incremental lift:** Calculated ROI is **182%**, proving paid ads deliver significant value when evaluated properly.  

---

## 🧪 Methodology  
This project uses causal inference techniques designed for observational data:  
- **Pre-post regression:** Initial benchmark comparing Google’s pre- and post-outage traffic.  
- **Parallel trends validation:** Confirmed Google and control platforms (Bing, Yahoo, Ask) had similar pre-treatment patterns.  
- **Difference-in-Differences (DiD):** Two-way fixed effects regression controlling for platform and time trends to estimate the true causal effect of ad suspension.  

---

## 🛠 Tools & Skills  
- **Language:** R  
- **Libraries:** `dplyr` (data wrangling), `ggplot2` (visualization), `plm` (panel regression)  
- **Techniques:** Causal inference, Difference-in-Differences, Panel Data Regression, ROI estimation  

---

## 🔗 Data Context  
- **Platform:** Bazaar.com (multi-channel e-commerce platform)  
- **Event:** Google’s sponsored search ads were paused for 3 weeks due to a technical glitch, while Bing, Yahoo, and Ask continued normal operations.  
- **Unit of Analysis:** Weekly branded search traffic (sponsored + organic) for each platform.  

---

## 📊 Results  
- **Traffic Impact:** DiD shows a **67% decrease** in Google’s branded traffic during the outage.  
- **Incremental ROI:** Adjusted ROI was **182%**, meaning $1 in ad spend generated $2.82 in revenue.  
- Clear divergence post-treatment validates the causal effect of ad suspension.  

---

## 📂 Repository Contents  
- **Analysis Report (PDF):** Detailed explanation of regression outputs, visualizations, and ROI calculations.  
- **R Scripts:**  
  - Data cleaning & transformation  
  - Traffic trend visualizations & parallel trends check  
  - Pre-post and DiD regression models  
  - ROI calculation from incremental lift  

---

## 🚀 Why This Matters  
This project demonstrates how applying **causal inference** to marketing data provides a realistic view of ad performance. By distinguishing incremental lift from organic fallback, it enables smarter budgeting decisions and avoids overestimating paid media value.  
