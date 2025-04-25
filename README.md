📚 GEOTWEETS-STOICISM-ANALYSIS

🚀 PROJECT OVERVIEW
This repository contains the complete pipeline and visualizations for analyzing the evolution of Stoicism-related discourse on Twitter using geotagged tweets collected between 2010 and 2023.
We leverage spatial and temporal analysis to track the presence and intensity of Stoic concepts and philosophical trends over time.

🎯 OBJECTIVES
- Identify and track the frequency of Stoicism-related keywords in geolocated tweets.
- Visualize temporal trends and thematic shifts across thirteen years.
- Provide structured outputs (datasets and charts) for further spatial, linguistic, and philosophical studies.

🗂️ DATA SOURCES
- Raw Data: Private geotagged Twitter datasets.
- Data Period: 2010–2023.
- Structure: TSV files with fields such as:
message_id, date, text, tags, tweet_lang, place, latitude, longitude, and more.

📌 Note: Due to data usage agreements, the original geotagged dataset is private and not publicly available.

🧠 KEYWORD FILTERING
The analysis uses two levels of keyword matching to ensure precision and coverage:

🔍 Wildcard Keywords (prefix matching):
altrui*, aristot*, cosmop*, epictet*, epicur*, eudaimon*, hedon*, philosoph*, plato*, pythago*, socrat*, stioc*, stoic*

🎯 Exact Keywords (exact word matching):
amorfati, aurelius, chrysippus, cicero, cleanthes, commongood, dichotomyofcontrol,
diogenes, hadot, humandignity, humanworth, jordanpeterson, mattis, mementomori,
moralinjury, moralaction, moralprogress, moralpurpose, musoniusrufus, nussbaum,
peripatetic, pigliucci, ryanholiday, seneca, stockdale, timferriss, zeno

This two-step strategy ensures comprehensive yet precise filtering of Stoic discourse without introducing unrelated topics.

🛠️ PIPELINE OVERVIEW
The workflow follows a structured five-stage process:
1. Data Loading 📥 — Load geotagged tweets year by year.
2. Keyword Filtering 🧹 — Apply wildcard and exact keyword filters.
3. Frequency Calculation 📊 — Aggregate yearly keyword frequencies.
4. Visualization 🎨 — Generate trendline graphs over time.
5. Output Generation 📄 — Export CSV datasets and visual outputs.

Full details are implemented in the Geotweets_Stoicism_Analysis_v5.ipynb notebook.

📦 OUTPUTS
keyword_frequencies_by_year.csv: Yearly keyword frequency dataset.
Four (4) trend graphs (PNG images) illustrating keyword evolution.
Jupyter Notebook containing the full reproducible pipeline.

🧩 HOW TO RUN
1. Clone the repository:
git clone https://github.com/cga-harvard/Geotweets-Stoicism-analysis.git
2. Open the Geotweets_Stoicism_Analysis_v5.ipynb notebook.
3. Adjust the data paths if necessary.
4. Execute all cells to reproduce the analysis.

⚙️ Requirements:
Python 3.11+
pandas
matplotlib
seaborn

Optimized for high-performance computing environments (HPC).

👨‍💻👩‍💻 AUTHORS
Rafael P. Albuquerque — Federal University of Rio Grande do Sul (UFRGS) | Visiting Scholar at Harvard CGA
Devika Jain — Harvard Center for Geographic Analysis (CGA)

🙏 ACKNOWLEDGMENTS
This research was conducted at the Harvard Center for Geographic Analysis (CGA).
Special thanks to the CGA research team and affiliated collaborators for their support.
