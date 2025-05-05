# Megaline Subscription Predictor

Proyecto del Sprint 9 del Bootcamp de Ciencia de Datos.  
El objetivo fue desarrollar un modelo de clasificación que prediga el plan más adecuado para cada cliente de la compañía Megaline con base en su comportamiento mensual.

---

## Descripción del Proyecto

Megaline quiere reemplazar sus planes heredados por dos nuevos planes: **Smart** y **Ultra**. Para apoyar esta transición, entrenamos un modelo que, con base en datos históricos del uso de llamadas, mensajes y datos móviles, recomienda el plan más apropiado para cada usuario.

---

## Datos utilizados

El dataset incluye información mensual de cada usuario:
- `calls`: número de llamadas realizadas
- `minutes`: minutos totales de llamadas
- `messages`: mensajes enviados
- `mb_used`: datos móviles usados en MB
- `is_ultra`: etiqueta objetivo (1 = Ultra, 0 = Smart)

---

## Modelos entrenados

- Árbol de Decisión (`DecisionTreeClassifier`)
- Bosque Aleatorio (`RandomForestClassifier`)
- Regresión Logística (`LogisticRegression`)

Se evaluaron distintos hiperparámetros (`max_depth`, `n_estimators`) para optimizar el rendimiento.

---

## Resultados

- Modelo seleccionado: **Random Forest**
- Exactitud en conjunto de prueba: **0.7527**
- Exactitud del modelo aleatorio (prueba de cordura): **0.4899**

---

## Librerías utilizadas

- Python 3.13.2
- pandas
- scikit-learn
- matplotlib
- numpy

---

## Estructura del repositorio

megaline-subscription-predictor/
│
├── users_behavior.csv
├── megaline_subscription_predictor.ipynb
├── env/
├── requirements.txt
├── README.md

## Cómo ejecutar este proyecto

Si deseas clonar este proyecto y ejecutarlo localmente, sigue estos pasos:

### 1. Clona el repositorio

```bash
git clone https://github.com/Marlene-Fraire/megaline-subscription-predictor.git
cd megaline-subscription-predictor


### 2. Crea y activa un entorno virtual

Con venv (opcional si usas conda):

```bash
python -m venv env
source env/bin/activate        # Mac/Linux
env\Scripts\activate           # Windows

O con `conda`:

```bash
conda create -n megaline_env python=3.13.2
conda activate megaline_env


### 3. Instala las dependencias

```bash
pip install -r requirements.txt


### 4. Abre el Notebook

```bash
jupyter notebook notebooks/megaline_subscription_predictor.ipynb


### Reproducibilidad
Este proyecto fue desarrollado con Python 3.13.2 y probado en entornos de Jupyter Notebook y VS Code. Si deseas garantizar resultados iguales, asegúrate de usar la misma versión de scikit-learn especificada en requirements.txt.


### Contacto
¿Tienes dudas, sugerencias o quieres compartir feedback?
Puedes encontrarme aquí: 
GitHub: https://github.com/Marlene-Fraire
LinkedIn: www.linkedin.com/in/diana-marlene-r-29109b83