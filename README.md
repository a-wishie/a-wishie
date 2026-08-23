# Hi, I'm Avishi.

I build systems that turn sustainability data into decisions.

B.Tech in Computer Science Engineering, SRM Institute of Science and Technology (CGPA 9.49/10.00)

I spent a year at MSCI Inc. on the Quantitative Index Research team. I started not knowing how to extract modular data. By the end, I was the person people came to when something did not reconcile, a methodology was not behaving as expected, or a check script needed to be built. I learned that ESG data is only as powerful as the analyst who can structure it, validate it, and communicate what it means. So I started building the tools I wished I had, and I open-sourced them.

## What I did at MSCI

I did not just run simulations. I repeatedly took a methodology document, rebuilt it independently in Python, and asked: does the implementation actually do what the methodology says?

- **Implemented and validated** 3 ETF-eligible thematic equity indexes end-to-end in Python and SQL, building backtesting and rebalancing logic from index methodologies and reconciling outputs against specifications.

- **Supported construction, validation, and operationalisation** of 20+ rules-based equity indexes across 7 institutional mandates, including one of the world's largest public pension funds, via QC scripting, methodology validation, and rebalance debugging across thematic and ESG-screened strategies.

- **Independently reconstructed** client equity index methodologies in Python to cross-validate production outputs, applying GICS-based sector segmentation and iterative constituent capping, then diagnosing mismatches between DSP, F9, and Workbench.

- **Built Python-based validation and analytics tooling** to verify index construction outputs, including cross-checks of daily price returns and ESG screening logic. I automated constituent extraction, QC analysis, tracking error calculation, and portfolio diagnostics.

- **Implemented** an iterative carbon-intensity reduction algorithm for an ESG-screened equity index, achieving a 30% GHG intensity reduction target vs. parent benchmark through rules-based exclusions.

- **Served as subject-matter expert** for an internal LLM-based thematic index research tool; developed a validation framework and guidelines adopted team-wide.

- **Investigated edge cases** that others missed: missing Scope 3 emissions before 2020, incorrect relevance-score mappings, opening vs. closing weight discrepancies, and climate-data gaps that caused securities to disappear from ESG indexes.

- **Worked directly with** Scope 1/2/3 emissions data, EVIC, carbon intensity calculations, projected emissions screens, LCT scores, ESG ratings, and controversy exclusions across Aware Super, GPIF, Thailand ESG, and ETF Connect projects.

- **Produced client-ready deliverables**: IMX reports, methodology slides, tracking error studies, and relative performance analysis for institutional clients and RFPs.

## What I'm building in the open

I believe the best way to learn sustainability analytics is to build, backtest, and publish. Here is what I have shipped so far:

**[ESG-Screener](https://github.com/a-wishie/ESG-Screener)** — Rules-based ESG screening on a 110-stock S&P 500 universe. Excluded 22 companies across 5 ESG criteria (fossil fuels, controversial weapons, high-carbon utilities, tobacco, gambling). The screened portfolio improved max drawdown by **341bps** and Sharpe ratio by **0.02** vs. unscreened, with **3.42%** tracking error.

**[Multi-Asset-Factor-Strategy](https://github.com/a-wishie/Multi-Asset-Factor-Strategy)** — Systematic multi-asset framework across US, European, and Japanese equities, layering factor selection, ESG overlay, and FX hedging. The ESG-Factor-Hedged variant delivered **17.31%** annualized return, **0.66** Sharpe, and **-29.17%** max drawdown. FX hedging alone added **163bps** annually by eliminating EUR and JPY drag.

**[SectNeut-Multi-Factor-Equity-Sim](https://github.com/a-wishie/SectNeut-Multi-Factor-Equity-Sim)** — Quality, value, and momentum factor index with sector-neutral constraints. Without neutralization, the portfolio concentrated **44%** in Financials. After neutralization, sector HHI dropped from **0.266** to **0.109**, volatility fell by **456bps**, and the information ratio improved from **0.67** to **0.92**.

**[Thematic-Index-Builder](https://github.com/a-wishie/Thematic-Index-Builder)** — MSCI-style thematic index construction with NLP relevance scoring, iterative issuer capping, and benchmark-relative analysis. Applied to clean energy with 23 keyword signals. Threshold sensitivity analysis showed stricter relevance filtering reduced underperformance by **158bps** in sector downturns.

**[DoomIndex](https://github.com/a-wishie/DoomIndex)** — Interactive disaster response dashboard with GeoJSON geographic visualization, Flask backend, React frontend, and Google Gemini LLM integration for civic guidance.

## How I work

- **Structure first.** Every project starts with a clear methodology document before a single line of code.
- **Validate everything.** I independently reconstruct production methodologies in Python to cross-check outputs. If the numbers do not match, I find out whether the issue is in the data, the methodology, or the implementation.
- **Communicate clearly.** Data is worthless if the decision-maker cannot act on it. I build dashboards, write READMEs, and package findings into formats that non-technical stakeholders can use.

## Tech Stack

Python, Pandas, NumPy, SQL, Excel (Advanced), Tableau, Git, Jupyter Notebook

## Let's connect

- [LinkedIn](https://linkedin.com/in/avishi14)
- [Email](mailto:avishi1404@gmail.com)
