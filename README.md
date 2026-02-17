<div align="center">

# 🔥 HR ATTRITION DASHBOARD 🔥
### *built in R · by Amit Kumar *

<br>

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![ggplot2](https://img.shields.io/badge/ggplot2-FF6B6B?style=for-the-badge&logo=r&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3D4F7C?style=for-the-badge&logo=plotly&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Status](https://img.shields.io/badge/status-submitted%20%26%20cooked-brightgreen?style=for-the-badge)

<br>

> *why are employees leaving? i made a whole interactive dashboard to find out.*
> *spoiler: overworking people is bad. who knew.*

</div>

---

<div align="center">

## 🎯 THE BIG QUESTION

</div>

```
does working 50+ hours a week   +   terrible work-life balance   =   people quitting?
```

**yes. obviously. but now i have charts to prove it.**

this project takes HR compensation data and breaks down employee attrition by:

<div align="center">

| 🕐 Hours Worked/Week | ⚖️ Work-Life Balance Score | 🧑 Gender |
|---|---|---|
| bucketed into ranges | scored 1–10, also bucketed | Male / Female / Other |
</div>
output is a **fully interactive HTML dashboard** — hover over any tile, get the exact numbers.



---

<div align="center">

## 💀 THE FINDING THAT BROKE MY BRAIN

</div>

<div align="center">

| Segment | Attrition Rate | Vibe |
|---|---|---|
| 😴 36–40 hrs + WLB score 8–10 | **5–11%** | ✅ chill, people are staying |
| 😟 Males, <35 hrs, low WLB | **40%** | ⚠️ something's wrong here |
| 💀 Males, 50+ hrs, WLB score 4–5 | **50%** | 🚨 half of them are GONE |

</div>

> **50% attrition.** that's not a data point. that's a fire alarm going off while HR makes a slide deck about "employee engagement initiatives."

the fix? let people go home. 36–40 hours + decent WLB = the sweet spot. groundbreaking stuff.

---

<div align="center">

## 🛠️ TECH STACK

</div>

```r
library(ggplot2)     # 🎨 the heatmap
library(plotly)      # ✨ made it interactive
library(dplyr)       # 🔧 data wrangling
library(tidyr)       # 🔧 reshaping
library(htmltools)   # 📦 built the full dashboard page
library(htmlwidgets) # 📦 exported everything to HTML
```

---

<div align="center">

## 🚀 HOW TO RUN IT

</div>

**step 1 — clone it**
```bash
git clone https://github.com/YOUR_USERNAME/hr-attrition-dashboard.git
cd hr-attrition-dashboard
```

**step 2 — install packages (once)**
```r
install.packages(c("ggplot2", "dplyr", "tidyr", "scales", "plotly", "htmlwidgets", "htmltools"))
```

**step 3 — run the script in RStudio**

you'll get three outputs:

| Output | What it is |
|---|---|
| `hr_attrition_dashboard.html` | 🌐 the full interactive dashboard — open in any browser |
| `hr_attrition_heatmap.png` | 🖼️ high-res static version, good for reports |
| `hr_attrition_heatmap.pdf` | 📄 PDF if your professor is old school |

---

<div align="center">

## 🗂️ PROJECT STRUCTURE

</div>

```
📁 hr-attrition-dashboard/
│
├── 📜 Assignment_Amit_kumar_D09.R      ← the whole script
├── 📊 hr_compensation.csv              ← raw HR data (input)
├── 🌐 hr_attrition_dashboard.html      ← open this in your browser
├── 🖼️  hr_attrition_heatmap.png        ← static plot
├── 📄 hr_attrition_heatmap.pdf         ← PDF version
└── 📝 README.md                        ← you're here
```

---

<div align="center">

## 📊 THE DASHBOARD

</div>

three heatmap panels — one per gender group. each tile = one hours/WLB combo.
the number on the tile = attrition %. hover it for the full breakdown.

```
🔵 blue          🟡 yellow          🔴 red
 low attrition ————————————> high attrition
    (good)                      (uh oh)
```

---

<div align="center">

## 💡 IF I HAD MORE TIME...

</div>

- 🔀 turned this into a **Shiny app** with department-level filters
- 📈 added a **time series chart** showing attrition trends over quarters
- 🤖 thrown in a **logistic regression model** to predict who's at risk next
- ✅ written actual unit tests *(lol)*

---

<div align="center">

---

**Amit Kumar** 

*February 2026*

*this was an assignment. i got way too into it.*

---

</div>
