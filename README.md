# 🚗 Predicción de Valores de Autos – Rusty Bargain

El servicio de venta de autos usados **Rusty Bargain** está desarrollando un modelo que determine el valor de mercado de cada vehículo. Para ello, se enfoca en:

- La calidad de la predicción  
- La velocidad de la predicción  
- El tiempo requerido para el entrenamiento  

## 🔍 Procesos

1. **Importación de Librerías**  
   Carga de Python y librerías necesarias.

2. **Preparación de Datos**  
   - **Importación de Datos:** Lectura del CSV original.  
   - **Datos Duplicados:** Identificación y eliminación de registros repetidos.  
   - **Datos Faltantes:**  
     - Análisis de columnas con valores nulos.  
   - **Tipos de Datos:** Conversión y normalización de formatos, especialmente fechas.  
   - **Datos Inconsistentes en el Target:** Detección y filtrado de valores atípicos o inválidos en la variable objetivo.  
   - **Eliminación de Columnas Vacías:** Remoción de columnas sin información relevante.  
   - **Codificación de Variables Categóricas:** Transformación a variables numéricas (one-hot encoding).  
   - **Estandarización:** Aplicación de `MinMaxdScaler` a las variables numéricas.  
   - **Separación Train/Test:** División del conjunto en datos de entrenamiento y prueba.

3. **Entrenamiento de Modelos**  
   - **Regresión Lineal**  
   - **Bosque Aleatorio**  
   - **LightGBM**  
   - **CatBoost**

4. **Análisis del Modelo**  
   - Comparación de todos los modelos en base a la métrica **RECM** (Raíz del Error Cuadrático Medio), tiempo de entrenamiento y número de hiperparámetros probados.  
   - Observaciones sobre la relación entre complejidad del modelo y reducción del error.  
   - Tabla comparativa de resultados y tiempos de entrenamiento.

## 🧰 Requisitos del Entorno
- Python 3.8 o superior
- pandas
- numpy
- scikit-learn
- matplotlib

## 🚀 Cómo Clonar este Repositorio

```bash
git clone https://github.com/dsc530/precio_vehiculos.git

