# Segmentación de clientes con Machine Learning — OnlineFoods

Análisis de datos y segmentación de clientes de una empresa de pedidos de alimentos en línea, usando K-Means clustering para apoyar la toma de decisiones estratégicas del negocio.

🔗 **[Ver demo en vivo →](https://vercel.com/giselle-leguizamo-s-projects/ml-analisis-pedidos-onlinefoods/9LnrGkuFTrb6oKXJkCV1ZXxSJzi8)**

---

## ¿Qué hace este proyecto?

A partir de una base de datos real de 388 clientes de la plataforma **OnlineFoods** (Bangalore, India), se implementó un algoritmo de aprendizaje no supervisado para:

- Identificar patrones de comportamiento en los clientes
- Segmentar la base en **3 grupos** según edad, ocupación, estado civil, ingresos y ubicación geográfica
- Generar recomendaciones de negocio personalizadas por grupo
- Predecir a qué grupo pertenece un cliente nuevo y asignarle un beneficio automáticamente

---

## Stack tecnológico

| Herramienta | Uso |
|---|---|
| Python | Lenguaje principal |
| Pandas | Limpieza y transformación de datos |
| Scikit-learn | Algoritmo K-Means |
| Matplotlib / Seaborn | Visualización de datos |
| Joblib | Exportación y reutilización del modelo |
| Google Colab | Entorno de desarrollo |

---

## Metodología

1. **Exploración y limpieza** — Se eliminaron columnas irrelevantes y 107 registros duplicados (de 388 → 281 únicos)
2. **Transformación** — Variables categóricas convertidas a numéricas (género, estado civil, ocupación, ingresos, feedback)
3. **Análisis exploratorio** — Gráficas de distribución por edad, género, ocupación, ingreso y ubicación geográfica
4. **Clustering K-Means** — Segmentación en 3 grupos con `n_clusters=3`, `random_state=42`
5. **Análisis geográfico** — Coordenadas de latitud/longitud mapeadas en Google Maps para identificar zonas de operación
6. **Implementación real** — Modelo exportado y probado con clientes nuevos para predicción de grupo y asignación de beneficios

---

## Resultados — Perfil de los 3 grupos

### Grupo 0 — Zona mixta (comercial + residencial)
- Edad promedio: 25 años
- Solteros, con ingresos bajos o medios
- **Beneficio asignado:** cupón por primera compra

### Grupo 1 — Zona comercial y universitaria (mayor concentración)
- Edad: 18–25 años, mayormente estudiantes
- Solteros, sin ingresos propios
- **Beneficio asignado:** promociones en productos top

### Grupo 2 — Zona residencial (segmento de oportunidad)
- Edad promedio: 30 años, casados
- Empleados, independientes o amas de casa
- **Beneficio asignado:** descuento del 5% + cupones en fechas especiales

---

## Conclusión principal

El cliente más frecuente es un joven de 23 años, soltero, estudiante, ubicado en la zona comercial del centro de Bangalore. Los mayores de 27 años en zonas residenciales representan un segmento sub-utilizado con alto potencial de crecimiento.

---

## Estructura del proyecto

```
ml-analisis-pedidos-onlinefoods/
├── TrabajoGrado_SeminarioMachineLearning_DarylGiselleLeguizamoRodriguez.ipynb
├── index.html                  # Demo interactivo (GitHub Pages)
└── README.md
```

## Contexto académico

Trabajo de grado · Seminario de Machine Learning en Tiempos de Datos  
Corporación Universitaria Remington · Facultad de Ingenierías · 2024  
Estudiante: Daryl Giselle Leguizamo Rodríguez

---

## Contacto
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Giselle%20Leguizamo-blue?logo=linkedin)](https://www.linkedin.com/in/giselleleguizamo)
[![GitHub](https://img.shields.io/badge/GitHub-dgzamo16-black?logo=github)](https://github.com/dgzamo16)
