# ⚽ 2022 FIFA World Cup Final: Passing Network & Centrality Analysis

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![StatsBomb](https://img.shields.io/badge/Data-StatsBomb-red)
![NetworkX](https://img.shields.io/badge/Library-NetworkX-green)
![mplsoccer](https://img.shields.io/badge/Library-mplsoccer-orange)

An end-to-end tactical data science project analyzing the passing structures and playmaker nodes of **Argentina** and **France** in the iconic **2022 FIFA World Cup Final** (Match ID: `3858949`), using StatsBomb open data.

---

## 📌 Executive Summary & Tactical Insights

By modeling event-level passing data into weighted directed graphs, this analysis quantifies how both finalists built their attack transitions:

* **🇦🇷 Argentina (Fluid & Central Playmaking):** 
  * High density of short-to-medium passes in the central midfield and attacking third.
  * **Lionel Messi** and **Enzo Fernández** recorded the highest **Betweenness Centrality** scores, proving mathematically that they acted as the primary tactical bridge between defense and attack.
* **🇫🇷 France (Vertical & Direct Transitions):** 
  * Passing architecture clustered around the defensive block and central defenders (**Raphaël Varane** & **Dayot Upamecano**).
  * High betweenness centrality in the backline highlights a low-block, rapid transition strategy targeting the wings (**Kylian Mbappé**).

---

## 📊 Visualizations

### 1. Passing Networks (mplsoccer)
| Argentina Pass Network | France Pass Network |
|:---:|:---:|
| ![Argentina Network](assets/argentina_pass_network.png) | ![France Network](assets/france_pass_network.png) |

> **Node size** represents total passes made; **line thickness** represents passing frequency between player pairs.

### 2. Betweenness Centrality Comparison (NetworkX)
![Centrality Comparison](assets/centrality_comparison.png)

---

## 🛠️ Tech Stack & Methodology

* **Data Extraction:** `statsbombpy` (StatsBomb Open Data)
* **Data Processing & Manipulation:** `pandas`, `numpy`
* **Network Graph Theory:** `networkx` (*Directed Graph, In-Degree & Betweenness Centrality*)
* **Sports Visualization:** `mplsoccer`, `matplotlib`

---

## 🚀 How to Run Locally / in Google Colab

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/fifa-2022-final-pass-network.git](https://github.com/YOUR_USERNAME/fifa-2022-final-pass-network.git)
   cd fifa-2022-final-pass-network
