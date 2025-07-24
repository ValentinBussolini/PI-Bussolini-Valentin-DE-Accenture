# 🛒 Proyecto Integrador 2025 - Bussolini (PI DE ACN)

Este repositorio contiene el desarrollo del Proyecto Integrador para el curso de Data Engineering en Accenture. El objetivo es diseñar y desplegar un sistema completo de gestión de datos orientado al análisis relacional y la modelación dimensional.

---

## 📁 Estructura del repositorio

```plaintext
PI Bussolini/
├── data/                # Archivos CSV originales (11 tablas)
├── notebooks/           # Notebook principal de análisis
│   └── PI 2025 DE ACN.ipynb
├── docker-compose.yml   # Definición del stack con PostgreSQL
├── requirements.txt     # Dependencias del entorno Python
├── readme.md            # Este documento

⚙️ Tecnologías utilizadas
Python (pandas, SQLAlchemy, psycopg2)

PostgreSQL (base de datos relacional)

Docker (orquestación del entorno)

Git + GitHub (versionado)

DBeaver (exploración de la base)

Jupyter Notebook (desarrollo y análisis técnico)

📥 Carga de datos
Los 11 archivos .csv se cargan automáticamente en sus respectivas tablas mediante un script con pandas.to_sql(). Se realiza una normalización previa de columnas (str.lower()) y se maneja la codificación con utf-8-sig.

🔍 Análisis exploratorio de calidad de datos
Se incluye una función analizar_nulos(tabla) que permite:

Detectar nulos estándar

Identificar nulos no reconocidos (ej. "null", "na", espacios)

Calcular porcentaje de nulos por columna

Visualizar totales y priorizar limpieza