# 🚕 Sweet Lift Taxi - Predicción de pedidos por hora

Este proyecto busca predecir la cantidad de pedidos de taxis para la siguiente hora en los aeropuertos, usando datos históricos de la compañía **Sweet Lift Taxi**. El modelo tiene como objetivo mejorar la disponibilidad de unidades en horas pico.

## 📊 Modelos usados

- Regresión Lineal
- Random Forest Regressor
- ARIMA

## 📈 Métrica

El modelo fue evaluado con **RMSE**. El mejor modelo logró una RMSE < 48 en el conjunto de prueba, cumpliendo los requisitos del proyecto.

## 🧠 Características del conjunto de datos

- Datos remuestreados por hora (`resample('1H')`)
- Variables rezagadas (`lag_1`, `lag_24`, etc.)
- Estacionalidad horaria y semanal
- Media móvil diaria

## 🔧 Herramientas y librerías

- Python 3.x
- pandas, numpy, matplotlib, statsmodels, scikit-learn

## 📁 Estructura

- `/notebooks`: notebook completo con el análisis
- `/images`: gráficas exportadas
- `requirements.txt`: instala todas las dependencias

## 🧪 Resultados

Modelo Random Forest Regressor logró el mejor desempeño:

| Modelo                  | RMSE |
|-------------------------|------|
| Random Forest Regressor | 43.6 |
| ARIMA                   | 47.8 |
| Regresión Lineal        | 56.2 |

## 🚀 Cómo ejecutarlo

1. Clona este repositorio:
   ```bash
   git clone https://github.com/cesardud/taxi_demand_prediction.git

2. Navega al proyecto:
   ```bash
   cd taxi_demand_prediction
   
3. Instala las librerías requeridas:
   ```bash
   pip install -r requirements.txt

4. Abre Notebook:
   ```bash
   jupyter notebook notebook.ipynb



