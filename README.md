# **Detección de Fraude en Transacciones con Tarjeta de Crédito**

### **Descripción**

Este proyecto utiliza algoritmos de Machine Learning para detectar transacciones fraudulentas con tarjetas de crédito. Se basa en el dataset de detección de fraude en tarjetas de crédito disponible en Kaggle.

## **Dataset**

Fuente: Kaggle - Credit Card Fraud Detection

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Tamaño: 284,807 transacciones

Clases:

0: Transacción normal

1: Transacción fraudulenta (0.1727% de los datos)

Variables: 30 (V1-V28 son variables anonimizadas, junto con Time y Amount)

## **Tecnologías Utilizadas**

-Python

-Pandas (para manipulación de datos)

-Matplotlib & Seaborn (visualización de datos)

-Scikit-learn (modelo de machine learning)

-Imbalanced-learn (SMOTE) (manejo del desbalanceo de datos)

## **Flujo del Proyecto**

Exploración y limpieza de datos

Análisis de distribuciones y correlaciones

Manejo del desbalanceo con SMOTE

Entrenamiento del modelo (Regresión Logística)

Evaluación del modelo

Guardado del modelo entrenado

## **Resultados del Modelo**

Accuracy: 98.85%

Precision (fraude): 99%

Recall (fraude): 94%

F1-score: 96%

## **Instalación y Uso**

Clona el repositorio:
```bash
git clone https://github.com/tu-usuario/credit-card-fraud-detection.git
cd credit-card-fraud-detection
```
Instala dependencias:
```bash
pip install -r requirements.txt
```
Ejecuta el código:

```bash
python fraud_detection.py
```
📂 Estructura del Proyecto

├── data
│   ├── creditcard.csv  # Dataset original
├── models
│   ├── fraud_detection_model.pkl  # Modelo entrenado
│   ├── scaler.pkl  # Escalador para normalizar datos
├── notebooks
│   ├── Exploratory_Data_Analysis.ipynb  # Análisis exploratorio
│   ├── Model_Training.ipynb  # Entrenamiento del modelo
├── src
│   ├── fraud_detection.py  # Script principal
├── README.md  # Este archivo
├── requirements.txt  # Librerías necesarias

📌 Notas

Se recomienda probar otros modelos como Random Forest o XGBoost para mejorar el recall en fraudes.

Ajustar hiperparámetros podría mejorar el rendimiento.
