# 🦠 COVID-19 South Africa: Data Analysis

A Jupyter Notebook analysis of South Africa's first 100 days of COVID-19, from the first confirmed case on **5 March 2020** to **12 June 2020**. It loads daily case data from JSON, cleans it with Pandas, and plots how the pandemic developed.

`Python` `Pandas` `NumPy` `Matplotlib` `Jupyter`

---

## 🗂️ Output

<img width="1368" height="685" alt="COVID-19 South Africa trends chart" src="https://github.com/user-attachments/assets/2eb83533-029c-4d01-906b-4cc13d47fca5" />

---

## 📊 The data

`covid.json` has 100 daily records with these fields:

| Field | Description |
|---|---|
| `Date` | Reporting date (2020/03/05 – 2020/06/12) |
| `Total Confirmed Cases` | Cumulative cases (61,927 by 12 June) |
| `Total Deaths` | Cumulative deaths (1,354) |
| `Total Recovered` | Cumulative recoveries (35,008) |
| `Active Cases` | Currently active cases (25,565) |
| `Daily Confirmed Cases` | New cases that day |
| `Daily  deaths` | New deaths that day |

---

## 🔍 What the notebook does

1. **Loads** the JSON file into a Pandas DataFrame
2. **Sorts** by date so the time series runs in order
3. **Converts types:** dates to `datetime` and case counts to numeric
4. **Plots** all six measures on one time-series chart, with labels, a title and a legend

---

## 📁 Project structure

```
Covid-analysis-project/
└── Python Files/
    ├── COVID ASSIGNMENT (1).ipynb   # Analysis notebook
    └── covid.json                   # Daily South African COVID-19 data
```

---

## 🔧 How to run

```bash
pip install pandas numpy matplotlib jupyter
cd "Python Files"
jupyter notebook "COVID ASSIGNMENT (1).ipynb"
```

Keep `covid.json` in the same folder as the notebook.

---

## 🚀 Next steps

- Remove the space thousand separators (e.g. `"61 927"`) before converting to numbers, so larger values aren't turned into `NaN`
- Plot cumulative and daily figures on separate charts, because the daily values are dwarfed by the totals
- Add a 7-day rolling average and the case fatality rate

---

## 🧠 What I learned

- Turning nested JSON into a clean DataFrame
- Working with time-series data and data types
- Designing a chart that tells a clear story

---

## 👩🏾‍💻 Author

**Sharon Galela** · [LinkedIn](https://www.linkedin.com/in/sharon-galela-6998bb265) · [GitHub](https://github.com/ShariieG)
