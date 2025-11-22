# **Stephen Jerge Ψ**  
**Clinical-Science–Track Researcher | Psychological Research Developer**

I build small, practical tools that support clinical and mental-health research—one-command runs that clean/de-ID data, flag issues, and leave a manifest.

**See it fast:** (Demo link here when recorded) — PRDT run with sample PHQ-9/GAD-7 data.

**Try it:**  
```bash
python3 -m venv .venv && source .venv/bin/activate
pip install https://github.com/stephenmjerge/psych-research-data-toolkit/releases/latest/download/prdt-0.1.4-py3-none-any.whl
prdt --config https://raw.githubusercontent.com/stephenmjerge/psych-research-data-toolkit/main/configs/anxiety.toml --outdir /tmp/prdt-demo
```
Outputs: clean/anonymized CSV, `alerts.json` (missingness/PHI/reliability), plots, and `run_manifest.json`.

---

## Core Projects (clinician-facing first)

1) [**PRDT — Psych Research Data Toolkit**](https://github.com/stephenmjerge/psych-research-data-toolkit)  
Clean + de-ID REDCap/Qualtrics exports; emit PHI quarantine, missingness/reliability alerts, plots, and a reproducible manifest.

2) [**MPAL — Mini Psychological Assessment Lab**](https://github.com/stephenmjerge/mini-psychological-assessment-lab)  
Scores PHQ-9, GAD-7, PCL-5, BDI-II; outputs severity labels, simple trends, and structured summaries for research/educational use.

3) [**PRWO — Psych Research Workflow Organizer**](https://github.com/stephenmjerge/psych-research-workflow-organizer)  
Weekly checklist + scripts that keep roadmaps/PortfolioHub/readmes in sync; posters workspace for artifacts before OSF upload.

4) [**ADOIF — Article / DOI Fetcher**](https://github.com/stephenmjerge/article-digital-object-identifier-fetcher)  
Pulls PDFs/metadata and organizes a review library for lit sweeps and faculty targeting.

5) [**RL-Sim — Reinforcement Learning Simulation**](https://github.com/stephenmjerge/reinforcement-learning-simulation)  
Tiny reward-learning simulations to link symptom severity and decision-making.

---

## Why this matters (for clinics/research)

- Safer handling: HMAC anonymization + PHI guardrails; data dictionaries and alerts to catch issues early.  
- Reproducible runs: manifests and configs per execution; tests run via `python -m pytest tests` (PRDT).  
- Clinician-ready outputs: cleaned CSVs, severity summaries, and plots that slot in after REDCap/Qualtrics and before SPSS/R.
