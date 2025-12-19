# NBA Home-Court Advantage Over Time  
### STAT 184 Final Project – Section 3  
### Authors: Charan Kuragayala, Rupin Reddy, Jayadeep Vadlapati

This repository contains a fully reproducible analysis of how **home-court advantage in the NBA has changed from 2000–2024**.  
We examine league-wide trends, decade-level patterns, and team-specific performance using **game-level historical NBA data**.

Our goal is to determine whether home-court advantage is **declining, stable, or evolving**, and to quantify these differences using win percentages, point differentials, and modern visualization methods.

---

## 🔍 Overview

Home-court advantage is a long-standing phenomenon in sports analytics.  
In this project, we:

- Compute home vs. away **win percentages** over 25 seasons  
- Track changes in **average point differential**  
- Compare teams across **three eras**: 2000s, 2010s, and 2020s  
- Visualize trends with line charts, heatmaps, and distribution plots  
- Identify which teams consistently outperform at home  

This analysis is fully reproducible using **Quarto**, **Tidyverse**, and the **nbastatR** package.

---

## ⭐ Interesting Insight

Across the 2000–2024 period, **league-wide home win percentage has steadily declined**, suggesting that home-court advantage is weaker today than it was two decades ago.  
Factors may include improved travel, analytics-driven game planning, and more efficient offensive systems.

(If required by rubric: include a saved PNG from `ggsave()` inside `figures/` and display it below.)

---

## 📊 Data Sources & Acknowledgements

This project uses publicly available and ethically sourced NBA game-level data:

- **Basketball Reference – Game Logs**  
  https://www.basketball-reference.com

- **OpenDataBay – NBA Scores & Betting Trends**  
  https://opendatabay.io  

- **NBA Stats API (Public Endpoint)**  
  https://stats.nba.com  

- **R package: nbastatR**  
  https://github.com/abresler/nbastatR  

### FAIR/CARE Alignment  
- **FAIR:** Data are findable (documented), accessible (open), interoperable (tidy format), and reusable.  
- **CARE:** Data involve no sensitive individual information and follow ethical public-use guidelines.

---

## 🛠 Reproducibility Instructions

To reproduce this project:

### 1️⃣ Install R, RStudio, and Quarto  
https://quarto.org/docs/get-started/

### 2️⃣ Install required R packages

```r
install.packages(c("tidyverse", "janitor", "gt", "scales", "lubridate", "purrr"))
remotes::install_github("abresler/nbastatR")
3️⃣ Open the main analysis file
bash
Copy code
analysis/final_project.qmd
4️⃣ Render the document
Click Render in RStudio

This will produce the final PDF in the same folder

This satisfies STAT 184’s Reproducible Workflow requirements.

📁 Repository Structure
nix
Copy code
.
├── analysis/
│   ├── final_project.qmd        # Main Quarto analysis file
│   ├── final_project.pdf        # Rendered final report
│
├── data/                        # Optional: store cached data if used
│
├── figures/                     # Saved plots (PNG/JPG) from ggsave()
│
├── scripts/                     # R scripts used during development
│
├── report/                      # Additional Quarto or LaTeX files if needed
│
├── Project_Guidelines.md        # Instructions from course template
├── README.md                    # Project documentation
└── .gitignore
This structure follows the official STAT 184 template and Open Science conventions.

🧠 Project Plan (PCIP-aligned)
Plan

Define research question

Locate and verify game-level NBA datasets

Code

Clean data

Compute home/away metrics

Produce descriptive statistics

Improve

Validate dataset

Adjust visualizations

Add decade classification

Polish

Finalize plots

Add captions and alt-text

Knit Quarto → PDF

Upload to GitHub with full version control

🧩 Version Control & Collaboration
This repository demonstrates:

Multiple commits from different authors

Use of branches

A completed pull request

Use of GitHub Issues for task management

Clear documentation and reproducible structure

This satisfies STAT 184’s Repro.4 and Repro.6 grading criteria.

👥 Authors
1) Rupin ReddyReddy
Email: rupinreddy27@gmail.com
GitHub: https://github.com/rupinreddy27-gif

2) Charan Kuragayala
Email: cmk6803@psu.edu
GitHub: https://github.com/charangit-22

3) Jayadeep Vadlapati
Email: jxv5302@psu.edu
GitHub: https://github.com/jayadeep0101
