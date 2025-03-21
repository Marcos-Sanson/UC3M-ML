[Version in Spanish/Castilian (versión en español/castellano)](./README-es.md)

# Machine Learning in Healthcare
# Universidad Carlos III de Madrid

This repository contains code, implementations, and reports for the **[Machine Learning in Healthcare](https://aplicaciones.uc3m.es/cpa/generaFicha?est=350&anio=2024&plan=392&asig=16803&idioma=2)** course at **[Universidad Carlos III de Madrid (UC3M)](https://www.uc3m.es/home)**, part of the **[Bachelor in Data Science and Engineering](https://www.uc3m.es/bachelor-degree/data-science)** program. Each lab focuses on advanced machine learning techniques tailored to real-world healthcare data, covering generative models, survival analysis, and point processes.

## Course Information
- **Course:** [Machine Learning in Healthcare (16803)](https://aplicaciones.uc3m.es/cpa/generaFicha?est=350&anio=2024&plan=392&asig=16803&idioma=2) 
- **Program:** [Bachelor in Data Science and Engineering](https://www.uc3m.es/bachelor-degree/data-science)
- **Institution:** [Universidad Carlos III de Madrid (UC3M)](https://www.uc3m.es/home)
- **Professors:**
  - **Dr. Pablo Martínez Olmos**: Associate Professor, Signal Theory and Communications Department
  - **Dr. Antonio Artés Rodríguez**: Professor, Signal Theory and Communications Department

## Collaborators/Students
This work is a collaborative effort from Marcos Sanson and Conrad Niewienda, under the guidance of the professors.

## Labs Overview

### Lab 1: Multi-View Variational Autoencoder (VAE) for MNIST-FMNIST
- **Objective:** Develop and analyze a multi-view Variational Autoencoder (VAE) to model MNIST and FashionMNIST datasets in a shared latent space, utilizing cross-domain generation. Each MNIST-FMNIST image pair is matched by category to enhance the VAE's ability to learn and generate meaningful representations.
- **Key Tasks:**
  - Implement a multi-view VAE to process paired datasets.
  - Generate cross-domain images, i.e., reconstruct FashionMNIST from MNIST images and vice versa.
  - Visualize the latent space using t-SNE and PCA to assess the VAE’s ability to learn coherent cross-view representations.
- **Report:** Includes model performance, observations on cross-domain generation, and a link to the code.
  - [UC3M-ML Lab 1 Implementing a Multi-View VAE for MNIST-FMNIST.pdf](./UC3M-ML%20Lab%201%20Implementing%20a%20Multi-View%20VAE%20for%20MNIST-FMNIST.pdf)  
- **Code:** 
  - [LAB01.ipynb](./LAB01.ipynb)

### Lab 2: Survival Analysis with Kaplan-Meier and Cox Regression
- **Objective:** Perform survival analysis on pediatric bone marrow transplant data. This lab aims to explore patient survival probabilities over time using Kaplan-Meier estimates and identify influential risk factors using Cox proportional hazards regression.
- **Key Tasks:**
  - Conduct exploratory data analysis (EDA) on patient features.
  - Cluster patients into groups based on relevant features (using K-Means or DBSCAN) and assess survival differences.
  - Compute survival functions for each cluster using Kaplan-Meier and Cox regression, interpreting Cox regression results to understand feature importance.
- **Report:** Summarizes survival function analysis, survival differences between groups, and provides an interpretative comparison of Kaplan-Meier and Cox methods. Includes a link to the code.
  - [UC3M-ML Lab 2 Survival Analysis.pdf](./UC3M-ML%20Lab%202%20Survival%20Analysis.pdf)  
- **Files:**
  - [LAB02.ipynb](./LAB02.ipynb) 

### Lab 3: Modeling Patient Event Data with Point Processes
- **Objective:** Apply point process modeling to analyze the timing and frequency of clinical events. Using Hawkes processes, this lab seeks to capture patterns in patient event data, such as recurring visits or treatments, and infer clinical insights from the model parameters.
- **Key Tasks:**
  - Cluster patients based on features and fit a Hawkes process model to each cluster.
  - Compare Hawkes process parameters across clusters to infer potential differences in event dynamics (e.g., frequency, triggers).
  - Discuss the clinical implications of the observed parameter variations, especially as they pertain to patient risk or healthcare utilization patterns.
- **Report:** Highlights differences between clusters in terms of point process parameters, along with clinical interpretations and a link to the code.
  - [UC3M-ML Lab 3 Point Processes.pdf](./UC3M-ML%20Lab%203%20Point%20Processes.pdf)  
- **Files:** 
  - [LAB03.ipynb](./LAB03.ipynb) 

### Automatic Atrium Segmentation Project
In addition to the three labs, this larger project focuses on developing machine learning algorithms for automatic 3D segmentation of the left atrium, particularly in patients with atrial fibrillation. The work includes preprocessing medical imaging data, building ML models, and evaluating segmentation results against manual annotations.

- **Project Poster**:  
  ![Poster Preview](Automatic_Atrium_Segmentation_Poster_Image.png)
- **PDF Version**: [Download Poster PDF](Automatic_Atrium_Segmentation_Poster.pdf)
- **PNG Version**: [Download Poster PNG](Automatic_Atrium_Segmentation_Poster_Image.png)

For more details, visit this repository: **[CardiologyML - Automatic Atrium Segmentation](https://github.com/officialconfuzius/cardiologyml)**.

## Usage
Each lab is provided as a Jupyter Notebook compatible with **Google Colab** for interactive execution. 

To run the labs:
1. **Download** or **clone** this repository.
2. Open each `.ipynb` file in Google Colab to view, edit, and execute the code interactively.
3. All necessary dependencies and libraries are detailed in each notebook's setup section.
