# NanozymeLab: Gamified Computational Modeling of Nanozyme Kinetics 
**Author:** [Anna Anandita](https://github.com/annaanandita) 

## Overview

**NanozymeLab** is an interactive, gamified web app for exploring and visualizing **nanozyme catalytic kinetics**.  
It combines **chemical modeling**, **Arrhenius temperature dependence**, and **pH-dependent enzyme activity** with a **game-based learning** interface.

The app lets users:
- Simulate enzyme-like nanozyme kinetics in real time 
- Adjust reaction parameters (temperature, pH, activation energy, enzyme loading)  
- Compete in built-in or custom **STEM challenges** 
- Visualize **heatmaps** of yield and rate surfaces  
- Receive **AI-style mentor feedback** based on performance  

---

## Features

| Category | Description |
|-----------|-------------|
| **Learn Mode** | Explore core nanozyme kinetics (E + S ⇌ ES → E + P) interactively. |
| **Play Mode** | Choose from preset or custom challenges; optimize your parameters and earn scores in real time. |
| **Explore Mode** | Generate parameter surfaces for yield vs. pH & temperature or v₀ vs. E_total & k₂ref. |
| **Mentor Tips** | The app gives feedback on catalytic efficiency and experimental design choices. |
| **Session History** | Track and compare attempts; export results for analysis. |

---

## Scientific Model

The model implements the reaction mechanism:

E + S ⇀↽ ES → E + P

with rate equations:

d[S]/dt = −k1[E][S] + k−1[ES]

d[ES]/dt = k1[E][S] − (k−1 + k2)[ES]

d[P]/dt = k2[ES]

and includes:
- **Arrhenius law** temperature dependence  
- **Bell-shaped pH activity** factor  
- Optional **competitive inhibition**  

---

## Installation

### 1. Clone the repository
git clone https://github.com/<your-username>/NanozymeLab.git
cd NanozymeLab

### 2. Create a virtual environment (recommended)
python3 -m venv env
source env/bin/activate

### 3. Install Repositories
pip install streamlit numpy scipy matplotlib

### 4. Run the app
From the project directory, run:
streamlit run nanozymelab.py
Streamlit will open a browser window automatically
→ typically at http://localhost:8501

## Game Instructions
Learn tab: Adjust reaction parameters and visualize concentration vs. time.
Play tab:
Choose a Built-in or Custom challenge
Press Start Game and tweak parameters in real time
Watch your Score and Mentor Tip update live
Explore tab: Generate surface plots of kinetic parameters.

## Educational Impact
This project bridges chemical kinetics, computational modeling, and STEM gamification, making it suitable for:
Undergraduate chemistry / materials science labs
Interactive teaching in nanozyme catalysis
Public STEM outreach and digital twin simulation training

## Citation
If you use this tool in research or teaching, please cite:
Anandita, A. (2025). NanozymeLab: Gamified Computational Modeling of Nanozyme Kinetics. GitHub Repository.

## Contributions are welcome! Please:
Fork the repo
Create a feature branch
Submit a pull request

## License
This project is released under the MIT License.

## Acknowledgments
Developed as part of an independent computational modeling initiative. 
Special thanks to the open-source scientific Python community.
