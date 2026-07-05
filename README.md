# 2026 FIFA World Cup Predictor 🏆

Live knockout-stage predictions powered by a hybrid Dixon-Coles Poisson + Elo model.

## Features
- **Auto-refresh** every 60 seconds (live badge updates)
- **10,000 Monte Carlo** tournament simulations → QF/SF/Final/title probabilities
- **Player-level xG** contributions from StatsBomb WC 2022 calibration
- **7 interactive charts**: Win prob, Tournament MC, Form Trajectory, Scoreline Heatmaps, Player xG Bubble, Goal Scoring Distribution, Golden Boot
- **Betting lines** (Decimal / American / Fractional) + value finder
- **Squad rosters** — real 2026 July squads for all 14 teams
- **Confirmed results** — France 1-0 Paraguay (Mbappé 70'), Morocco 3-0 Canada

## APIs Used
- **Zafronix** (`https://api.zafronix.com/docs`) — tournament data, squads
- **Ball Don't Lie** (`https://api.balldontlie.io/fifa/worldcup/v1`) — teams, matches
- **StatsBomb Open Data** — WC 2022 shot-level xG calibration

## Run Locally
```bash
git clone https://github.com/Infurni09/worldcup-predictor.git
cd worldcup-predictor
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Deploy to Streamlit Community Cloud
1. Fork or connect this repo at https://share.streamlit.io
2. Set main file: `streamlit_app.py`
3. Add secrets in Advanced Settings (see `.streamlit/secrets.toml.template`)
