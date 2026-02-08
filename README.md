bellabeat-case-study/
│
├── README.md
├── LICENSE (optional)
│
├── notebook/
│   ├── bellabeat_case_study.ipynb
│   └── bellabeat_case_study.Rmd   (optional)
│
├── data/
│   ├── raw/
│   │   ├── dailyActivity_merged.csv
│   │   ├── sleepDay_merged.csv
│   │   └── hourlySteps_merged.csv
│   │
│   └── processed/
│       └── activity_sleep.csv
│
├── scripts/
│   ├── 01_load_packages.R
│   ├── 02_import_data.R
│   ├── 03_clean_data.R
│   ├── 04_join_data.R
│   ├── 05_analysis.R
│   └── 06_visualizations.R
│
├── outputs/
│   ├── figures/
│   │   ├── steps_vs_sedentary.png
│   │   ├── sleep_vs_time_in_bed.png
│   │   ├── steps_vs_sleep.png
│   │   └── activity_distribution.png
│   │
│   └── tables/
│       ├── summary_statistics.csv
│       ├── user_type_percent.csv
│       └── daily_average.csv
│
└── docs/
    ├── bellabeat_case_study_report.pdf
    └── bellabeat_case_study_slides.pdf (optional)
