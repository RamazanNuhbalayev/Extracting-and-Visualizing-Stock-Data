# Stock & Revenue Dashboard

> **Track Tesla and GameStop at a glance — then dive as deep as you like.**
> A single Jupyter-notebook project that pairs share-price history with quarterly revenue so *anyone* can spot patterns, while tech-savvy users can tweak the code in minutes.

---

## 1 Why This Matters *(Business View)*

Financial headlines change daily, but numbers tell the real story. By placing **price** and **performance** side by side, the dashboard helps:

* **Investors** gauge whether earnings growth justifies today’s market price.
* **Managers & analysts** illustrate narratives with clear, shareable visuals.
* **Students & enthusiasts** explore real-world data without drowning in jargon.

*(Scroll down for a 2-minute “Run it yourself” guide.)*

---

## 2 What You’ll See

| Insight                                   | Example View                                                  |
| ----------------------------------------- | ------------------------------------------------------------- |
| **Historical share price** (5-year range) | 📈 Line chart highlighting big swings and milestones.         |
| **Quarterly revenue**                     | 💰 Bar chart showing how earnings evolve over time.           |
| **Price ↔ Revenue overlay**               | 🔄 One click to compare market reactions with actual results. |

Add screenshots (`assets/`) to showcase the visuals on LinkedIn.

---

## 3 Quick Start *(No Coding Required)*

1. **Download or clone** the repo from GitHub.
2. Double-click `Start_Dashboard.bat` *(Windows)* or run `bash start_dashboard.sh` *(macOS/Linux)*.
3. Your browser opens the notebook; hit **Run All** → interactive charts appear.

> *The script takes care of Python, libraries, and launching Jupyter automatically.*

---

## 4 For Developers & Data Scientists

| Step                         | Command / File                                               | Notes                     |
| ---------------------------- | ------------------------------------------------------------ | ------------------------- |
| Create venv                  | `python -m venv venv`                                        | Optional but recommended. |
| Activate venv                | `source venv/bin/activate`  (`venv\Scripts\activate` on Win) |                           |
| Install deps                 | \`\`\`bash                                                   |                           |
| pip install yfinance==0.2.38 |                                                              |                           |
| pip install pandas==2.2.2    |                                                              |                           |
| pip install plotly           |                                                              |                           |
| pip install beautifulsoup4   |                                                              |                           |

```
| Versions pinned for reproducibility. |
| Launch Jupyter | `jupyter notebook` | Open `Stock_Revenue_Dashboard.ipynb`. |

**Tech stack:** Python · Pandas · Plotly · BeautifulSoup · Yahoo Finance API (`yfinance`)

### 4.1 How the Notebook Works
1. **Pull prices** via `yfinance.download()` (daily granularity).  
2. **Scrape revenue** tables from Investor Relations pages using BeautifulSoup.  
3. **Clean & merge** datasets into a tidy `DataFrame`.  
4. **Plotly Express** renders interactive line & bar charts.  
5. **Dash export** *(optional)*—run `python to_dash.py` to spin up a standalone web app.

---

## 5 Road-map Ideas
- [ ] Auto-refresh data with GitHub Actions  
- [ ] Add margin, EPS & free-cash-flow visuals  
- [ ] Deploy on Streamlit / HuggingFace Spaces

Pull requests are welcome — fork, branch, code, and open a PR! 🚀

---

## 6 Credits & Contact
Created by **Ramazan Nuhbalayev** — connect on [LinkedIn](https://www.linkedin.com/) or open an issue for questions.

---

> *Empower your feed with data you can actually use — whether you’re a curious reader or a power user.*
```
