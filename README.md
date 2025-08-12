# 📊 Análisis de Componentes Principales (PCA)

Este proyecto implementa **Análisis de Componentes Principales (PCA)** para explorar y reducir la dimensionalidad de un conjunto de datos, destacando las variables que más contribuyen a la varianza total.

---

## 🧠 Objetivo
El propósito es:
- 🔍 **Descubrir patrones ocultos** en los datos.
- 📉 **Reducir variables** manteniendo la mayor varianza posible.
- 📊 **Visualizar** relaciones entre variables en un espacio reducido.

---

## ⚙️ Tecnologías utilizadas
| Herramienta      | Uso principal |
|------------------|--------------|
| **Python 3**     | Lenguaje principal |
| **Pandas**       | Manipulación de datos |
| **NumPy**        | Cálculo numérico |
| **Scikit-learn** | Implementación de PCA |
| **Matplotlib** / **Seaborn** | Visualización de datos |

---

## 🔄 Flujo del análisis
1. 📥 **Carga** del dataset.
2. 🧹 **Preprocesamiento**: limpieza y escalado de variables.
3. 🧮 **Cálculo de PCA** con `scikit-learn`.
4. 📈 **Visualización** de la varianza explicada.
5. 🗂 **Interpretación** de *loadings* y componentes.

---

## 📈 Resultados principales
- Se identificaron las **componentes principales** que explican la mayor parte de la varianza.
- Las **variables clave** en cada componente fueron determinadas mediante *loadings*.
- Visualizaciones que muestran la distribución y relación de los datos en el nuevo espacio PCA.

Ejemplo de gráfico de varianza explicada:

![Varianza Explicada](docs/varianza_explicada.png)

Ejemplo de proyección en dos componentes principales:

![Proyección PCA](docs/proyeccion_pca.png)

---

## 📂 Estructura del repositorio
```
├── Análisis_de_PCA.ipynb   # Notebook con el análisis completo
├── README.md               # Este archivo
└── docs/
    ├── varianza_explicada.png
    └── proyeccion_pca.png
```

---

## 🚀 Ejecución
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
jupyter notebook Análisis_de_PCA.ipynb
```

---

**Autor:** *Tu Nombre*  
📅 **Fecha:** 2025  
📧 **Contacto:** tu.email@ejemplo.com

---
