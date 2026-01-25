# Solar Power Generation Forecasting

Machine learning-based solar energy forecasting system using the Anikannal Solar Power Generation Dataset.

## Features

- Time-series forecasting with weather data
- Model comparison (Linear Regression vs Random Forest)
- Interactive Streamlit web interface
- Temporal feature engineering (lag, rolling mean)

## Dataset

- **Source**: Anikannal Solar Power Generation Dataset (Plant 1)
- **Generation Data**: 15-minute intervals
- **Weather Data**: Hourly measurements
- **Merge Strategy**: Time-aware merge using `merge_asof`

## Quick Start

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Train Models
```bash
python train_model.py
```

### 3. Run Streamlit App
```bash
streamlit run app.py
```

## Models

### Linear Regression (Baseline)
- MAE: ~16.80
- RMSE: ~32.10

### Random Forest (Final Model)
- MAE: ~16.75
- RMSE: ~32.04

## Project Structure

```
new_aiml/
├── app.py                      # Streamlit web app
├── train_model.py              # Model training script
├── requirements.txt            # Dependencies
├── linear_model.pkl            # Trained Linear Regression
├── random_forest_model.pkl     # Trained Random Forest
├── feature_names.pkl           # Feature list
└── README.md                   # Documentation
```

## Features Used

1. **Weather Features**: Ambient Temperature, Module Temperature, Irradiation
2. **Temporal Features**: Hour, Month, Day of Week
3. **Lag Features**: Previous AC Power (lag_1)
4. **Rolling Features**: 3-period rolling mean

## Methodology

1. **Data Preprocessing**: Time-aware merge, remove night periods (AC_POWER = 0)
2. **Feature Engineering**: Extract temporal features + lag/rolling features
3. **Train-Test Split**: 80-20 chronological split (no shuffle)
4. **Model Training**: Linear Regression + Random Forest
5. **Evaluation**: MAE & RMSE metrics

## Deployment

Deploy on Streamlit Cloud:
1. Push to GitHub
2. Connect repository to Streamlit Cloud
3. Deploy with one click

## Author

Built for AI/ML Course Project

## License

Educational Project
