# 🏀 When Does the Clock Start Ticking?  
### Exploring Scoring Peaks in the NBA and WNBA  

**UC San Diego – COGS 108 Final Project**  
By: Justice Loyola, Palak Gupta, Reva Agrawal, Peiling Cheng, Noah Mirano  

📺 [Watch Project Video](https://drive.google.com/file/d/18Rrw9eavpvJga57bSeuL7HbONwHvIDwL/view?usp=drive_link)  

---

## 📌 Overview  
This project investigates the relationship between **player age** and **scoring impact** in the NBA and WNBA, exploring how athletes’ contributions evolve throughout their careers. Using large-scale datasets from **Basketball Reference** and **FiveThirtyEight**, we created a custom **Scoring Impact Metric** (proportion of a player’s points to their team’s total points) and analyzed league-wide trends across age, gender, and league structures.  

Our findings reveal that while NBA players peak in their **late 20s**, WNBA players tend to peak **later** and sustain performance longer — reflecting league-specific differences in workload, playing style, and physical demands.  

---

## 🔍 Research Question  
How does a basketball player’s **age** influence their **scoring contribution** to their team, and how do these trajectories differ between the **NBA** and **WNBA**?  

---

## ⚡ Key Insights  
- **NBA players peak at ~27 years old**, followed by a gradual decline in scoring impact.  
- **WNBA players peak closer to 35 years old**, with more sustained contributions later in their careers.  
- League structures (season length, physical intensity, development pathways) significantly affect performance longevity.  
- The **Scoring Impact Metric** provides a transparent, intuitive way to measure a player’s direct contribution, compared to composite metrics like PER or Win Shares.  

---

## 📊 Features & Methods  
- **Data Acquisition**: Collected NBA and WNBA player/team data from Basketball Reference & FiveThirtyEight.  
- **Data Cleaning & Preprocessing**:  
  - Dropped null values, standardized team & player identifiers.  
  - Converted percentages to numeric fields and normalized metrics.  
  - Merged player-level and team-level datasets across 20k+ observations.  
- **Custom Metric Development**:  
  - **NBA**: Estimated total points via `Points per 36 × Games Played`.  
  - **WNBA**: Estimated points via `Usage Rate × Minutes Played`.  
  - Normalized against team totals for per-season contribution %.  
- **Exploratory Data Analysis**:  
  - LOWESS smoothing to reveal non-linear age trends.  
  - Binned means for clear peak/decline visualization.  
  - Comparative boxplots across age groups and leagues.  
- **Statistical Modeling**:  
  - Identified peak ages using grouped averages.  
  - Applied linear regression to estimate post-peak decline rates.  

---

## 🛠 Tech Stack  
- **Languages**: Python (Pandas, NumPy)  
- **Visualization**: Matplotlib, Seaborn, Statsmodels (LOWESS)  
- **Data Sources**:  
  - [NBA Player Stats (FiveThirtyEight)](https://github.com/fivethirtyeight/nba-player-advanced-metrics/blob/master/nba-data-historical.csv)  
  - [NBA Team Stats (Basketball Reference)](https://www.basketball-reference.com/teams/)  
  - [WNBA Player Stats (FiveThirtyEight)](https://github.com/fivethirtyeight/WNBA-stats/blob/master/wnba-player-stats.csv)  
  - [WNBA Team Stats (Basketball Reference)](https://www.basketball-reference.com/wnba/teams/)  

---

## 💡 Skills Demonstrated  
- **Data Wrangling & Cleaning**: handled large, messy historical sports data.  
- **Feature Engineering**: developed custom metrics for player impact.  
- **Statistical Analysis**: applied regression & smoothing methods to detect trends.  
- **Visualization & Storytelling**: created clear, engaging plots for technical + non-technical audiences.  
- **Team Collaboration**: coordinated roles across data, analysis, visualization, and interpretation.  

---

## 📈 Results  
- **NBA Peak Age**: 27.0 years  
  - Decline rate: ~0.17 percentage points per year (statistically significant).  
- **WNBA Peak Age**: 35.0 years  
  - Decline rate: ~0.69 percentage points per year (not statistically significant).  
- WNBA players sustain scoring impact **longer** than NBA players on average.  
- Younger WNBA players often take **larger roles earlier** in their careers compared to NBA rookies.  

---


## 🎯 Why This Project Matters  
This project demonstrates the ability to:  
- Translate **raw, unstructured sports data** into **actionable insights**.  
- Build **custom metrics** that reveal patterns hidden by traditional statistics.  
- Combine **statistical rigor** with **visual storytelling** to answer real-world questions.  

Beyond basketball, this approach showcases skills directly applicable to **business analytics, data science, and intelligence roles**:  
- Identifying **key performance metrics**  
- Measuring **impact over time**  
- Communicating **complex data stories** clearly to stakeholders  

---

## 📜 License  
Open-source for educational and portfolio use.  

---

## ☕ About Me

Hi! I’m **Palak Gupta**, a Mathematics–Computer Science student with a deep interest in data analytics, business intelligence, and data engineering. I enjoy building real-world projects that combine technical skill with business insight, using tools like SQL, Docker, Notion, and automation platforms like n8n.

📫 **Let’s connect**:  
- 🔗 [LinkedIn](https://www.linkedin.com/in/palakgupta28/)  
- 📧 [palakgupta0428@gmail.com](mailto:palakgupta0428@gmail.com)  

---



