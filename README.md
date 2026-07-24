# 🐍 Proyecto Lógica: Katas de Python

## 📝1. Descripción del Proyecto
Este repositorio reúne la resolución de **40 Katas de programación en Python** (serie de 41 ejercicios con la Kata 35 omitida por falta de enunciado en el temario original.
El proyecto fue diseñado como un entrenamiento intensivo de lógica algorítmica y programación funcional, evolucionando desde la manipulación básica de variables hasta el modelado de reglas de negocio. Todo el código fue construido bajo **estándares de calidad de nivel de producción:** manejo explícito de errores, documentación uniforme, uso de módulos nativos de la librería estándar y salidas formateadas dinámicamente para entornos interactivos en **VS Code**.

## 🏗️2. Estructura del Repositorio
La organización del proyecto se estructuró de manera modular dividiendo la serie de Katas en 4 Jupyter Notebooks temáticos para facilitar su navegación, ejecución y auditoría:
```text
proyecto_katas_python/
 │
 ├── DataProject/
 │    └── EnunciadoDataProjectPython.pdf  # Enunciado original de Katas a resolver
 │
 ├── NotebooksJupyter/
 │    ├── katas_1_10.ipynb     # Katas 1 a 10: Sintaxis base, cadenas y matemáticas
 │    ├── katas_11_20.ipynb    # Katas 11 a 20: Listas, bucles y lógica condicional
 │    ├── katas_21_30.ipynb    # Katas 21 a 30: Colecciones, diccionarios y funciones
 │    └── katas_31_41.ipynb    # Katas 31 a 41: Funcional (reduce), datetime, unpacking   │                               y reglas de negocio (sin Kata 35)
 │
 └── README.md                 # Documentación técnica del proyecto
```
## 📈3. Estándares Técnicos y Convenciones de Código
Para mantener una cohesión absoluta a lo largo de los 40 ejercicios, se definió y respetó una arquitectura de código estricta:
•	**Docstrings Estandarizados (Sin typing importado)**: Tipeado descriptivo en minúsculas en el encabezado de cada función (int | float, str, tuple), manteniendo el código liviano y legible.
•	**Programación Defensiva (try/except + isinstance):** Ninguna función rompe la ejecución si recibe datos corruptos. Todas validan rangos y tipos de datos de entrada devolviendo mensajes descriptivos ante excepciones *(ValueError, TypeError)*.
•	**Trazabilidad Interna (# CONSIGNA):** Comentarios numerados dentro del cuerpo de las funciones para mapear la solución paso a paso contra los requerimientos.
•	**Formateo Tabular Avanzado:** Uso de *f-strings* con especificadores de alineación *({var:<10})* y formato de precisión *({var:.2f})*.
•	**Control Dinámico de Impresión:** Verificación de tipos mediante *isinstance(resultado, (int, float))* para diferenciar respuestas numéricas exitosas de cadenas de error, evitando fallos de formateo en consola.
