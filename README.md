# Dengue Forecast — Santiago de Cali

Sistema de pronóstico y alerta temprana de dengue a nivel ciudad,
comparando modelos estadísticos, Machine Learning y Deep Learning.

## Contexto
Serie temporal semanal 2015–2024. Cali reportó 38.009 casos en 2024,
73% por encima de la incidencia nacional.

## Modelos evaluados
| Familia       | Modelos                                    |
|---------------|--------------------------------------------|
| Estadísticos  | MA, ETS (Holt-Winters), ARIMA, SARIMA, SARIMAX, Prophet |
| ML            | XGBoost, LightGBM, Random Forest, Gradient Boosting     |
| Deep Learning | MLP, LSTM, TCN (PyTorch)                   |

## Mejor modelo
XGBoost — MAE: 8.87 · RMSE: 11.53 · MAPE: 4.71%
Validado con ventana rodante de 30 iteraciones con parada temprana.

## Estructura
PROYECTO_GRADO/
├── data/               ← no incluido (.gitignore)
├── mc_barrios/         ← no incluido (.gitignore)
├── versionfinal.ipynb  ← notebook principal
└── xgb_feature_importance.csv


## Nota
Los datos originales (.parquet y .shp) no están incluidos por su tamaño y sensibilidad.