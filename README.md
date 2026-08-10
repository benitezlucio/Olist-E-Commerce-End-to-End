#  Olist E-Commerce End-to-End Data Science Project

Este repositorio contiene un análisis de datos de extremo a extremo (*End-to-End*) utilizando el dataset público de **Olist**, la plataforma de e-commerce más grande de Brasil. El proyecto abarca desde la exploración e ingesta de datos hasta la limpieza, análisis exploratorio (EDA), ingeniería de características y el desarrollo de modelos de Machine Learning.

---

## 📌 Tabla de Contenidos
1. [Descripción del Proyecto](#-descripción-del-proyecto)
2. [Flujo de Trabajo (Pipeline)](#-flujo-de-trabajo-pipeline)
3. [Tecnologías Utilizadas](#-tecnologías-utilizadas)
4. [Instalación y Uso](#-instalación-y-uso)
5. [Resultados y Conclusiones](#-resultados-y-conclusiones)

---

## 🎯 Descripción del Proyecto

El objetivo principal de este proyecto es analizar el comportamiento de compras, tiempos de entrega, satisfacción de clientes y ventas en el ecosistema de Olist para extraer *insights* de negocio clave y construir modelos predictivos aplicados a Machine Learning.

**Preguntas clave del proyecto:**
* ¿Qué factores influyen principalmente en la puntuación de las reseñas (*review scores*)?
* ¿Cómo impactan los tiempos de logística en la satisfacción del cliente?
* ¿Se puede predecir el comportamiento del cliente o segmentar su valor dentro de la plataforma?

---

🔄 Flujo de Trabajo (Pipeline)
El desarrollo del proyecto se estructuró en 4 fases principales:

Comprensión de Datos (01_Data_Understanding.ipynb): Inspección de esquemas, relaciones relacionales entre tablas de Olist y validación del alcance de cada variable.

Limpieza de Datos (02_Data_Cleaning.ipynb): Tratamiento de datos faltantes, deduplicación, conversión de formatos de fecha/hora y corrección de tipos de datos.

Análisis Exploratorio (EDA.ipynb): Visualización de métricas de ventas, distribución geográfica de compradores/vendedores, análisis de logística e impacto del flete en la puntuación de las órdenes.

Machine Learning (ML_Models+Conclusions.ipynb): Selección e ingeniería de características, evaluación de algoritmos predictivos, optimización de hiperparámetros y síntesis de hallazgos para la toma de decisiones.

🛠️ Tecnologías Utilizadas
Lenguaje: Python 3.x

Manipulación de datos: Pandas, NumPy

Visualización: Matplotlib, Seaborn

Machine Learning: Scikit-Learn

Entorno de desarrollo: JupyterLab / Visual Studio Code

🚀 Instalación y Uso
Clonar el repositorio:

Bash
git clone [https://github.com/benitezlucio/Olist-E-Commerce-End-to-End.git](https://github.com/benitezlucio/Olist-E-Commerce-End-to-End.git)
cd Olist-E-Commerce-End-to-End
Crear y activar un entorno virtual (opcional pero recomendado):

Bash
python -m venv venv
# En Windows:
venv\Scripts\activate
# En macOS/Linux:
source venv/bin/activate
Instalar dependencias necesarias:

Bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
Ejecutar los notebooks:

Bash
jupyter notebook
📊 Resultados y Conclusiones
El modelo permite identificar aproximadamente 47 de cada 100 experiencias que terminarían siendo negativas. De las experiencias que el modelo señala como potencialmente negativas, aproximadamente 56 de cada 100 efectivamente presentan una valoración negativa. Esto permite priorizar clientes potencialmente insatisfechos para acciones de seguimiento, aceptando cierto nivel de falsas alertas..

Los tiempos de envío muestran una correlación directa con las calificaciones negativas (reviews de 1 y 2 estrellas).

Los modelos evaluados permitieron clasificar la satisfacción del cliente con métricas sólidas de evaluación.
