[Version in English (versión en inglés)](./README.md)

# Aprendizaje Automático en Salud
# Universidad Carlos III de Madrid

Este repositorio contiene código, implementaciones e informes para el curso **[Aprendizaje Automático en Salud](https://aplicaciones.uc3m.es/cpa/generaFicha?est=350&anio=2024&plan=392&asig=16803&idioma=2)** en la **[Universidad Carlos III de Madrid (UC3M)](https://www.uc3m.es/home)**, parte del programa **[Grado en Ciencia e Ingeniería de Datos](https://www.uc3m.es/bachelor-degree/data-science)**. Cada laboratorio se centra en técnicas avanzadas de aprendizaje automático aplicadas a datos de salud del mundo real, cubriendo modelos generativos, análisis de supervivencia y procesos puntuales.

## Información del Curso
- **Curso:** [Aprendizaje Automático en Salud (16803)](https://aplicaciones.uc3m.es/cpa/generaFicha?est=350&anio=2024&plan=392&asig=16803&idioma=2) 
- **Programa:** [Grado en Ciencia e Ingeniería de Datos](https://www.uc3m.es/bachelor-degree/data-science)
- **Institución:** [Universidad Carlos III de Madrid (UC3M)](https://www.uc3m.es/home)
- **Profesores:**
  - **Dr. Pablo Martínez Olmos:** Profesor Asociado, Departamento de Teoría de la Señal y Comunicaciones
  - **Dr. Antonio Artés Rodríguez:** Catedrático, Departamento de Teoría de la Señal y Comunicaciones

## Colaboradores/Estudiantes
Este trabajo es un esfuerzo colaborativo de Marcos Sanson y Conrad Niewienda, bajo la guía de los profesores.

## Resumen de Laboratorios

### Laboratorio 1: Autoencoder Variacional Multi-Vista (VAE) para MNIST-FMNIST
- **Objetivo:** Desarrollar y analizar un Autoencoder Variacional Multi-Vista (VAE) para modelar los conjuntos de datos MNIST y FashionMNIST en un espacio latente compartido, utilizando generación cruzada. Cada par de imágenes MNIST-FMNIST está emparejado por categoría para mejorar la capacidad del VAE de aprender y generar representaciones significativas.
- **Tareas Clave:**
  - Implementar un VAE multi-vista para procesar conjuntos de datos emparejados.
  - Generar imágenes cruzadas, es decir, reconstruir FashionMNIST a partir de imágenes MNIST y viceversa.
  - Visualizar el espacio latente utilizando t-SNE y PCA para evaluar la capacidad del VAE de aprender representaciones coherentes de vista cruzada.
- **Informe:** Incluye rendimiento del modelo, observaciones sobre la generación cruzada y un enlace al código.
  - [UC3M-ML Lab 1 Implementación de un VAE Multi-Vista para MNIST-FMNIST.pdf](./UC3M-ML%20Lab%201%20Implementing%20a%20Multi-View%20VAE%20for%20MNIST-FMNIST.pdf)
- **Código:** 
  - [LAB01.ipynb](./LAB01.ipynb)

### Laboratorio 2: Análisis de Supervivencia con Kaplan-Meier y Regresión de Cox
- **Objetivo:** Realizar un análisis de supervivencia en datos de trasplante de médula ósea pediátrica. Este laboratorio busca explorar las probabilidades de supervivencia de los pacientes a lo largo del tiempo utilizando estimaciones de Kaplan-Meier e identificar factores de riesgo influyentes mediante la regresión de Cox.
- **Tareas Clave:**
  - Realizar un análisis exploratorio de datos (EDA) en las características de los pacientes.
  - Agrupar a los pacientes en grupos basados en características relevantes (usando K-Means o DBSCAN) y evaluar las diferencias de supervivencia.
  - Calcular funciones de supervivencia para cada grupo utilizando Kaplan-Meier y regresión de Cox, interpretando los resultados de la regresión de Cox para comprender la importancia de las características.
- **Informe:** Resumen del análisis de la función de supervivencia, diferencias de supervivencia entre grupos y una comparación interpretativa de los métodos de Kaplan-Meier y Cox.
  - [UC3M-ML Lab 2 Análisis de Supervivencia.pdf](./UC3M-ML%20Lab%202%20Survival%20Analysis.pdf)
- **Archivos:**
  - [LAB02.ipynb](./LAB02.ipynb)

### Laboratorio 3: Modelado de Datos de Eventos Clínicos con Procesos Puntuales
- **Objetivo:** Aplicar el modelado de procesos puntuales para analizar la temporalidad y frecuencia de eventos clínicos. Utilizando procesos de Hawkes, este laboratorio busca capturar patrones en los datos de eventos de pacientes, como visitas recurrentes o tratamientos, e inferir insights clínicos a partir de los parámetros del modelo.
- **Tareas Clave:**
  - Agrupar a los pacientes basándose en características y ajustar un modelo de procesos de Hawkes para cada grupo.
  - Comparar los parámetros de los procesos de Hawkes entre grupos para inferir posibles diferencias en la dinámica de los eventos (por ejemplo, frecuencia, desencadenantes).
  - Discutir las implicaciones clínicas de las variaciones observadas en los parámetros, especialmente en relación con el riesgo del paciente o los patrones de utilización de servicios de salud.
- **Informe:** Destaca las diferencias entre los grupos en términos de parámetros de procesos puntuales, junto con interpretaciones clínicas y un enlace al código.
  - [UC3M-ML Lab 3 Procesos Puntuales.pdf](./UC3M-ML%20Lab%203%20Point%20Processes.pdf)
- **Archivos:** 
  - [LAB03.ipynb](./LAB03.ipynb)

### Proyecto de Segmentación Automática del Atrio
Además de los tres laboratorios, este proyecto más amplio se centra en desarrollar algoritmos de aprendizaje automático para la segmentación automática en 3D del atrio izquierdo, particularmente en pacientes con fibrilación auricular. El trabajo incluye el preprocesamiento de datos de imágenes médicas, la construcción de modelos de ML y la evaluación de resultados de segmentación frente a anotaciones manuales.

Para más detalles, visite este repositorio: **[CardiologyML - Segmentación Automática del Atrio](https://github.com/officialconfuzius/cardiologyml)**.

## Uso
Cada laboratorio se proporciona como un cuaderno de Jupyter compatible con **Google Colab** para su ejecución interactiva. 

Para ejecutar los laboratorios:
1. **Descargue** o **clone** este repositorio.
2. Abra cada archivo `.ipynb` en Google Colab para visualizar, editar y ejecutar el código de forma interactiva.
3. Todas las dependencias necesarias se detallan en la sección de configuración de cada cuaderno.
