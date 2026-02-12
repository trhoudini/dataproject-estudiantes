🧠 Data Project sobre Machine Learning: Rendimiento Académico de Estudiantes


📖 Descripción del Proyecto  
Este proyecto forma parte de un trabajo de análisis de datos sobre Machine Learning y tiene como objetivo analizar el rendimiento académico de estudiantes. Para ello se realiza lo siguiente:

- Entender qué variables influyen más en la nota final (EDA).
- Preparar los datos para Machine Learning (preprocesamiento).
- Predecir una variable numérica mediante regresión (predicción de `nota_final`).
- Predecir una variable binaria mediante clasificación (predicción de `aprobado`).

El proyecto se apoya en un dataset principal (`dataset_estudiantes.csv`).

Principales técnicas aplicadas:
- Limpieza y transformación de datos con Pandas.
- Visualización con Matplotlib y Seaborn.
- Análisis estadístico descriptivo y correlaciones.
- Codificación de variables categóricas (One-Hot / Target Encoding según el caso).
- Entrenamiento y evaluación de modelos de Regresión y Clasificación.

Dataset y Variables: 
El dataset recoge información académica y hábitos del estudiante. Variables del proyecto:

- `horas_estudio_semanal`: Número de horas de estudio a la semana.
- `nota_anterior`: Nota que obtuvo el alumno en la convocatoria anterior.
- `tasa_asistencia`: Tasa de asistencia a clase en porcentaje.
- `horas_sueno`: Promedio de horas que duerme el alumno al día.
- `edad`: Edad del alumno.
- `nivel_dificultad`: Dificultad del alumno para el estudio.
- `tiene_tutor`: Indica si el alumno tiene tutor o no.
- `horario_estudio_preferido`: Horario de estudio preferido por el alumno.
- `estilo_aprendizaje`: Forma de estudio que emplea el alumno.
- `nota_final`: Calificación final obtenida por el estudiante.
- `aprobado`: Variable objetivo binaria que indica si el estudiante aprueba.


📁 Estructura del Proyecto  
├── 01-EDA.ipynb                           # Análisis exploratorio (EDA)  
├── 02-Preproceso.ipynb                    # Preprocesamiento y preparación de datos  
├── 03-Regresión.ipynb                     # Entrenamiento y validación del modelo de regresión  
├── 04-Clasificación.ipynb                 # Entrenamiento y validación del modelo de clasificación  
│  
├── dataset_estudiantes.csv                # Dataset original  
├── dataset_estudiantes_EDA.csv            # Dataset preparado/limpio para análisis  
├── df_regresion.csv                       # Dataset final para regresión  
├── df_clasificacion.csv                   # Dataset final para clasificación  
│  
├── modelo_regresion.pkl                   # Modelo entrenado (regresión)  
├── modelo_clasificacion.pkl               # Modelo entrenado (clasificación)  
│  
├── .gitignore  
└── README.md  


🛠 Instalación y Requisitos  
Proyecto desarrollado en Python por VSCode.

Paquetes a instalar recomendados para su realización:

pip install numpy pandas matplotlib seaborn scikit-learn category_encoders

Notas:
- `scikit-learn` lo usamos para modelos y transformaciones (escalado, OneHot, etc.).
- `category_encoders` lo usamos si se aplica Target Encoding en algunas variables categóricas.


📌 Resultados y Conclusiones
- El proyecto permite entender qué factores se relacionan más con la nota final y con aprobar. Variables como `nota_anterior` y `tasa_asistencia` suelen aparecer como factores fuertes para estimar la nota.
- La regresión ayuda a estimar una nota aproximada (no exacta), detectando patrones generales.
- La clasificación permite detectar probabilidad de aprobar, pero hay que vigilar el desbalanceo de clases.
- Los modelos guardados (`.pkl`) permiten reutilizar lo entrenado sin re-entrenar.


🔄 Próximos Pasos  
- Probar más modelos (modelos de algoritmos avanzados, árboles de decisión, RandomForest, XGBoost).
- Ajustar hiperparámetros con GridSearch / RandomSearch.
- Tratar el desbalanceo de `aprobado` (class_weight, SMOTE, etc.).
- Crear una pequeña “app” o script para predecir con nuevos estudiantes.


🤝 Contribuciones  
Si te interesa mejorar o extender este proyecto, las contribuciones son bienvenidas.


✒ Autor  
Autor: Francisco Troyano Martínez  
Contacto: troyano1406@gmail.com  
GitHub: https://github.com/trhoudini  
