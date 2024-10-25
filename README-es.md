[English Version of README](./README.md)

# Aprendizaje Automático en Salud (Universidad Carlos III de Madrid)

Este repositorio contiene código, implementaciones e informes para el curso **[Aprendizaje Automático en Salud](https://aplicaciones.uc3m.es/cpa/generaFicha?est=350&anio=2024&plan=392&asig=16803&idioma=2)** en la **[Universidad Carlos III de Madrid (UC3M)](https://www.uc3m.es/home)**, parte del programa **[Grado en Ciencia e Ingeniería de Datos](https://www.uc3m.es/bachelor-degree/data-science)**. Cada laboratorio se centra en técnicas avanzadas de aprendizaje automático aplicadas a datos de salud del mundo real, cubriendo modelos generativos, análisis de supervivencia y procesos puntuales.

## Información del Curso
- **Curso:** [Aprendizaje Automático en Salud (16803)](https://aplicaciones.uc3m.es/cpa/generaFicha?est=350&anio=2024&plan=392&asig=16803&idioma=2) 
- **Programa:** [Grado en Ciencia e Ingeniería de Datos](https://www.uc3m.es/bachelor-degree/data-science)
- **Institución:** [Universidad Carlos III de Madrid (UC3M)](https://www.uc3m.es/home)
- **Instructor:** Profesor Pablo Martínez Olmos

## Resumen de Laboratorios

### Laboratorio 1: Autoencoder Variacional Multi-Vista (VAE) para MNIST-FMNIST
- **Objetivo:** Desarrollar y analizar un Autoencoder Variacional Multi-Vista (VAE) para modelar los conjuntos de datos MNIST y FashionMNIST en un espacio latente compartido, utilizando la generación cruzada. Cada par de imágenes MNIST-FMNIST está emparejado por categoría para mejorar la capacidad del VAE de aprender y generar representaciones significativas.
- **Tareas Clave:**
  - Implementar un VAE multi-vista para procesar conjuntos de datos emparejados.
  - Generar imágenes cruzadas, es decir, reconstruir FashionMNIST a partir de imágenes MNIST y viceversa.
  - Visualizar el espacio latente utilizando t-SNE y PCA para evaluar la capacidad del VAE de aprender representaciones coherentes de vista cruzada.
- **Informe:** Incluye el rendimiento del modelo, observaciones sobre la generación cruzada y un enlace al código.
- **Archivos:** 
  - [LAB01.ipynb](./LAB01.ipynb)

### Laboratorio 2: Análisis de Supervivencia con Kaplan-Meier y Regresión de Cox
- **Objetivo:** Realizar un análisis de supervivencia en datos de trasplante de médula ósea pediátrica. Este laboratorio busca explorar las probabilidades de supervivencia de los pacientes a lo largo del tiempo utilizando estimaciones de Kaplan-Meier e identificar factores de riesgo influyentes mediante la regresión de Cox.
- **Tareas Clave:**
  - Realizar un análisis exploratorio de datos (EDA) en las características de los pacientes.
  - Agrupar a los pacientes en grupos basados en características relevantes (usando K-Means o DBSCAN) y evaluar las diferencias de supervivencia.
  - Calcular funciones de supervivencia para cada grupo utilizando Kaplan-Meier y regresión de Cox, interpretando los resultados de la regresión de Cox para comprender la importancia de las características.
- **Informe:** Resumen del análisis de la función de supervivencia, diferencias de supervivencia entre grupos y una comparación interpretativa de los métodos de Kaplan-Meier y Cox. Incluye un enlace al código.
- **Archivos:**
  - [LAB02.ipynb](./LAB02.ipynb)

### Laboratorio 3: Modelado de Datos de Eventos de Pacientes con Procesos Puntuales
- **Objetivo:** Aplicar el modelado de procesos puntuales para analizar el tiempo y la frecuencia de eventos clínicos. Usando procesos de Hawkes, este laboratorio busca capturar patrones en los datos de eventos de los pacientes, como visitas o tratamientos recurrentes, e inferir conocimientos clínicos a partir de los parámetros del modelo.
- **Tareas Clave:**
  - Agrupar a los pacientes en función de características y ajustar un modelo de proceso de Hawkes a cada grupo.
  - Comparar los parámetros del proceso de Hawkes entre grupos para inferir posibles diferencias en la dinámica de eventos (por ejemplo, frecuencia, desencadenantes).
  - Discutir las implicaciones clínicas de las variaciones observadas en los parámetros, especialmente en lo que se refiere al riesgo del paciente o a los patrones de utilización de la atención sanitaria.
- **Informe:** Resalta las diferencias entre los grupos en términos de parámetros del proceso puntual, junto con interpretaciones clínicas y un enlace al código.
- **Archivos:** 
  - (Próximamente)

## Uso
Cada laboratorio se proporciona como un Jupyter Notebook compatible con **Google Colab** para su ejecución interactiva. Para ejecutar los laboratorios:
1. **Descargar** o **clonar** este repositorio.
2. Abrir cada archivo `.ipynb` en Google Colab para ver, editar y ejecutar el código de forma interactiva.
3. Todas las dependencias y bibliotecas necesarias están detalladas en la sección de configuración de cada notebook.
