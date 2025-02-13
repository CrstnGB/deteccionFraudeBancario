# Detección de fraude en movimientos transaccionales con Deep Learning

## Descripción del Proyecto
Este proyecto aborda el desafío de la **detección de fraudes bancarios en línea**, un problema crítico en el contexto actual de la banca digital. El objetivo principal es aplicar técnicas de **deep learning** para identificar transacciones fraudulentas, contribuyendo a la seguridad en el sector financiero.

### Criterios de Éxito
- **Alta tasa de detección de fraudes** (sensibilidad > 80%).
- **Precisión moderada**, permitiendo una mayor tolerancia a falsos positivos. (precision )
- **Exactitud general alta**, asegurando un equilibrio entre la detección de fraudes y la minimización de errores.

---

## Objetivos

### Objetivo General
Desarrollar un sistema de detección de fraudes utilizando técnicas de **deep learning** que logre una alta efectividad en la identificación de transacciones fraudulentas.

### Objetivos Específicos
1. Seleccionar y preparar un **dataset** adecuado para el entrenamiento de modelos.
2. Realizar un **Análisis Exploratorio de Datos (EDA)** para comprender las características del conjunto de datos.
3. Eliminar variables redundantes y transformar los datos para su uso en redes neuronales.
4. Evaluar la utilidad de técnicas de **clusterización** en la detección de fraudes.
5. Implementar y comparar modelos de **deep learning**, incluyendo:
   - Redes Neuronales Densas (**DNN**).
   - Redes Neuronales Convolucionales (**CNN**).
   - Un modelo combinado **DNN + CNN**.
6. Convertir instancias tabulares en **pseudo-imágenes** mediante transformaciones matriciales para el entrenamiento de la CNN.
7. Alcanzar una **tasa de detección superior al 80%** sin comprometer la exactitud general del sistema.

---

## Metodología

### 1. Selección del Dataset
Se ha seleccionado un dataset representativo de transacciones bancarias, que incluye tanto transacciones legítimas como fraudulentas. El dataset ha sido cuidadosamente analizado y preparado para su uso en modelos de deep learning.

### 2. Análisis Exploratorio de Datos (EDA)
Se ha realizado un **EDA** exhaustivo para:
- Comprender la distribución de las clases (fraude vs. no fraude).
- Identificar y eliminar variables redundantes.
- Transformar los datos para su uso en redes neuronales.

### 3. Transformación de Datos
- **Conversión a pseudo-imágenes**: Para el entrenamiento de la CNN, las instancias tabulares se han transformado en matrices (pseudo-imágenes) mediante técnicas de **transformación matricial**.

### 4. Modelos Implementados
- **Red Neuronal Densa (DNN)**: Un modelo clásico de deep learning para datos tabulares.
- **Red Neuronal Convolucional (CNN)**: Aprovecha la estructura de las pseudo-imágenes para detectar patrones complejos.
- **Modelo Combinado (DNN + CNN)**: Combina las predicciones de ambos modelos para mejorar la efectividad.

### 5. Evaluación de Modelos
Los modelos se han evaluado utilizando métricas clave como:
- **AUC-ROC**: Para medir la capacidad de discriminación entre clases.
- **Sensibilidad (Recall)**: Para evaluar la tasa de detección de fraudes.
- **Exactitud (Accuracy)**: Para medir el rendimiento general del sistema.

---

## Resultados

Los resultados obtenidos indican que los modelos **DNN** y **CNN** combinados han cumplido con los criterios establecidos:
- **AUC-ROC > 80%**: Alta capacidad de discriminación entre transacciones fraudulentas y legítimas.
- **Sensibilidad > 80%**: Efectividad en la detección de fraudes.
- **Exactitud alta**: Equilibrio entre la detección de fraudes y la minimización de errores.

---

## Código y Recursos

El código implementado para este proyecto está disponible en este repositorio. Incluye:
- **Preprocesamiento de datos**.
- **Implementación de modelos** (DNN, CNN y combinado).
- **Evaluación de resultados**.

**El archivo del código se encuentra en: code/Detec_fraud_mov_trans_deepL_v7.ipynb**

### Requisitos
- Python 3.12.7
- Bibliotecas: requirements.txt

### Instalación
1. Clona el repositorio:
   ```bash
   git clone https://github.com/CrstnGB/deteccion-fraudes.git