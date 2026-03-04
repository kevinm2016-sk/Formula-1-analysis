# Formula 1 2008 Season – Data Analysis with Python

**Tools:** Python, Google Colab, CSV  
**Program:** Master in Data Analytics – ProfessionAI

---

## What's this about

This is my first Python project — I had zero programming background before starting the Master, so this was genuinely built from scratch after going through the course material twice.

The dataset covers the 2008 Formula 1 season. I used it to build three functions that calculate driver performance, generate a standings file, and rank constructors — all using base Python without any external libraries like Pandas.

---

## What I built

**Function 1 – Driver Performance**  
Takes a driver's name as input and returns their total points, wins, and podiums across the season. Points are calculated using the 2008 scoring system (10-8-6-5-4-3-2-1).

Example output for Hamilton:
```
Punti: 98
Vittorie: 5
Podi: 10
```

**Function 2 – Driver Standings to .txt**  
Loops through all drivers in the dataset, calculates their season points, and writes the full standings to a `Drivers_Standings_2008.txt` file.

**Function 3 – Constructor Standings**  
Same logic applied at team level — aggregates points by constructor and prints the ranked standings.

2008 Constructor results from the dataset:
```
Ferrari:   172
McLaren:   151
BMW:       135
Renault:    61
Toyota:     56
Toro Rosso: 35
```

---

## How I approached it

The data is loaded from a CSV file into a list of dictionaries using Python's built-in `csv.DictReader` — no Pandas, just standard library. Each function then iterates through that list and applies the scoring logic.

The functions are intentionally straightforward and a bit repetitive — I was still getting comfortable with loops, conditionals, and dictionaries at this stage. The constructor standings sorting came from a Colab autocomplete suggestion that I understood and kept.

---

## Files

- `progetto_analisi_f1.ipynb` — Jupyter notebook (runs on Google Colab)
- `formula1_data.csv` — source dataset (needs to be added to Google Drive if running the notebook)

---

*Part of my ongoing Data Analytics portfolio. More projects coming.*
