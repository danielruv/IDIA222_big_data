# Students Performance — Análisis y Preprocesamiento de Datos

Proyecto individual de la actividad **ED.01.02. Git, GitHub y reproducibilidad**
(Manejo Masivo de Datos — IDIA222-4, UPQ).

## Descripción

Análisis exploratorio (EDA) y preprocesamiento del dataset
[Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
de Kaggle (1000 estudiantes, calificaciones de matemáticas, lectura y escritura).

## Estructura del proyecto

```
student-performance-analysis/
├── data/
│   ├── StudentsPerformance.csv            # dataset original
│   └── StudentsPerformance_procesado.csv  # dataset preprocesado (generado)
├── notebooks/
│   └── analisis_preprocesamiento.ipynb    # EDA + preprocesamiento
├── requirements.txt
├── .gitignore
└── README.md
```

## Pasos que sigue el notebook

1. Importar los datos.
2. Exploración inicial (filas, columnas, tipos de dato).
3. Revisión de duplicados.
4. Revisión de valores nulos.
5. Distribución de las variables categóricas.
6. Distribución de las calificaciones.
7. Detección de outliers con el método IQR.
8. Columna nueva: promedio de calificaciones.
9. Codificación de variables categóricas (`get_dummies`).
10. Exportar el dataset preprocesado.

## Cómo reproducirlo

1. Clonar el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd student-performance-analysis
   ```
2. Crear y activar un entorno virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate      # Windows: venv\Scripts\activate
   ```
3. Instalar las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
4. Ejecutar el notebook:
   ```bash
   jupyter notebook notebooks/analisis_preprocesamiento.ipynb
   ```

## Autor

Daniel Ruvalcaba Juárez — Matrícula 126058326
Ingeniería en Datos e Inteligencia Artificial — UPQ

## Resultados
- El promedio general de calificaciones ronda los 65-70 puntos. - Se detectaron algunos outliers en math score, calificaciones muy bajas.