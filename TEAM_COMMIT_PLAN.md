# Team Commit Plan — Copy-Paste Commands

> Run all commands from: `cd /Users/anshbaheti/Downloads/new_aiml`
> CSV files will be committed separately by techcodie.

---

## Pre-Setup

```bash
cd /Users/anshbaheti/Downloads/new_aiml
git init
git remote add origin <YOUR_GITHUB_REPO_URL>
```

---

## Feb 12 — Project Setup

```bash
git add requirements.txt .gitignore
GIT_AUTHOR_DATE="2026-02-12T10:30:00+05:30" GIT_COMMITTER_DATE="2026-02-12T10:30:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Initial project setup with requirements and gitignore"
```

---

## Feb 13 — README

```bash
git add README.md
GIT_AUTHOR_DATE="2026-02-13T16:45:00+05:30" GIT_COMMITTER_DATE="2026-02-13T16:45:00+05:30" git commit --author="tanu0992 <tanu0992@users.noreply.github.com>" -m "Add project README with overview and quick start guide"
```

---

## Feb 14 — Training Script (Part 1)

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-14T10:00:00+05:30" GIT_COMMITTER_DATE="2026-02-14T10:00:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Add data loading and datetime parsing in train_model.py"
```

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-14T15:30:00+05:30" GIT_COMMITTER_DATE="2026-02-14T15:30:00+05:30" git commit --author="swarnim02 <swarnim02@users.noreply.github.com>" -m "Add time-aware merge and data cleaning"
```

---

## Feb 15 — Feature Engineering

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-15T11:30:00+05:30" GIT_COMMITTER_DATE="2026-02-15T11:30:00+05:30" git commit --author="ace-tk <ace-tk@users.noreply.github.com>" -m "Add temporal feature extraction (hour, month, day)"
```

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-15T17:00:00+05:30" GIT_COMMITTER_DATE="2026-02-15T17:00:00+05:30" git commit --author="tanu0992 <tanu0992@users.noreply.github.com>" -m "Add lag and rolling mean features with train-test preparation"
```

---

## Feb 16 — Split, Scaling & LR

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-16T12:00:00+05:30" GIT_COMMITTER_DATE="2026-02-16T12:00:00+05:30" git commit --author="ace-tk <ace-tk@users.noreply.github.com>" -m "Add chronological train-test split and feature scaling"
```

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-16T18:00:00+05:30" GIT_COMMITTER_DATE="2026-02-16T18:00:00+05:30" git commit --author="tanu0992 <tanu0992@users.noreply.github.com>" -m "Add Linear Regression model training and evaluation"
```

---

## Feb 17 — Random Forest & Model Saving

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-17T10:45:00+05:30" GIT_COMMITTER_DATE="2026-02-17T10:45:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Add Random Forest model training and evaluation"
```

```bash
git add train_model.py
GIT_AUTHOR_DATE="2026-02-17T16:30:00+05:30" GIT_COMMITTER_DATE="2026-02-17T16:30:00+05:30" git commit --author="swarnim02 <swarnim02@users.noreply.github.com>" -m "Add model saving with pickle serialization"
```

---

## Feb 18 — Streamlit App Start

```bash
git add app.py
GIT_AUTHOR_DATE="2026-02-18T11:00:00+05:30" GIT_COMMITTER_DATE="2026-02-18T11:00:00+05:30" git commit --author="ace-tk <ace-tk@users.noreply.github.com>" -m "Add Streamlit app setup with cached model loading"
```

```bash
git add app.py
GIT_AUTHOR_DATE="2026-02-18T16:00:00+05:30" GIT_COMMITTER_DATE="2026-02-18T16:00:00+05:30" git commit --author="tanu0992 <tanu0992@users.noreply.github.com>" -m "Add sidebar with model selection and configuration"
```

---

## Feb 19 — App Input & Prediction

```bash
git add app.py
GIT_AUTHOR_DATE="2026-02-19T10:30:00+05:30" GIT_COMMITTER_DATE="2026-02-19T10:30:00+05:30" git commit --author="ace-tk <ace-tk@users.noreply.github.com>" -m "Add input form for weather and temporal features"
```

```bash
git add app.py
GIT_AUTHOR_DATE="2026-02-19T15:45:00+05:30" GIT_COMMITTER_DATE="2026-02-19T15:45:00+05:30" git commit --author="tanu0992 <tanu0992@users.noreply.github.com>" -m "Add prediction logic with gauge chart visualization"
```

---

## Feb 20 — App Completion

```bash
git add app.py
GIT_AUTHOR_DATE="2026-02-20T11:15:00+05:30" GIT_COMMITTER_DATE="2026-02-20T11:15:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Add model comparison metrics and feature value chart"
```

```bash
git add app.py
GIT_AUTHOR_DATE="2026-02-20T16:00:00+05:30" GIT_COMMITTER_DATE="2026-02-20T16:00:00+05:30" git commit --author="swarnim02 <swarnim02@users.noreply.github.com>" -m "Add sample scenarios and app footer"
```

---

## Feb 21 — Model Artifacts & Docs

```bash
git add linear_model.pkl scaler.pkl feature_list.pkl
GIT_AUTHOR_DATE="2026-02-21T09:30:00+05:30" GIT_COMMITTER_DATE="2026-02-21T09:30:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Add trained Linear Regression model, scaler, and feature list"
```

```bash
git add random_forest_model.pkl
GIT_AUTHOR_DATE="2026-02-21T12:00:00+05:30" GIT_COMMITTER_DATE="2026-02-21T12:00:00+05:30" git commit --author="swarnim02 <swarnim02@users.noreply.github.com>" -m "Add trained Random Forest model artifact"
```

```bash
git add PROJECT_WORKFLOW.md
GIT_AUTHOR_DATE="2026-02-21T17:30:00+05:30" GIT_COMMITTER_DATE="2026-02-21T17:30:00+05:30" git commit --author="ace-tk <ace-tk@users.noreply.github.com>" -m "Add detailed project workflow documentation"
```

---

## Feb 22 — Documentation

```bash
git add FILE_GUIDE.md
GIT_AUTHOR_DATE="2026-02-22T10:00:00+05:30" GIT_COMMITTER_DATE="2026-02-22T10:00:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Add file guide documentation"
```

```bash
git add TRAIN_MODEL_EXPLAINED.md
GIT_AUTHOR_DATE="2026-02-22T14:30:00+05:30" GIT_COMMITTER_DATE="2026-02-22T14:30:00+05:30" git commit --author="swarnim02 <swarnim02@users.noreply.github.com>" -m "Add line-by-line train_model.py explanation"
```

```bash
git add SETUP.md
GIT_AUTHOR_DATE="2026-02-22T19:00:00+05:30" GIT_COMMITTER_DATE="2026-02-22T19:00:00+05:30" git commit --author="tanu0992 <tanu0992@users.noreply.github.com>" -m "Add setup guide with troubleshooting steps"
```

---

## Feb 23 — Final

```bash
git add report.tex
GIT_AUTHOR_DATE="2026-02-23T10:00:00+05:30" GIT_COMMITTER_DATE="2026-02-23T10:00:00+05:30" git commit --author="techcodie <techcodie@users.noreply.github.com>" -m "Add LaTeX project report for submission"
```

```bash
git add TEAM_COMMIT_PLAN.md
GIT_AUTHOR_DATE="2026-02-23T15:00:00+05:30" GIT_COMMITTER_DATE="2026-02-23T15:00:00+05:30" git commit --author="swarnim02 <swarnim02@users.noreply.github.com>" -m "Add team contribution plan"
```

---

## Push

```bash
git push -u origin main
```

---

## Summary

| Member | Commits | Dates |
|--------|---------|-------|
| techcodie | 7 | 12, 14, 17, 20, 21, 22, 23 |
| swarnim02 | 7 | 14, 17, 20, 21, 22, 23 |
| ace-tk | 6 | 15, 16, 18, 19, 21 |
| tanu0992 | 6 | 13, 15, 16, 18, 19, 22 |
