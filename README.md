# Generative Modelling Case Study using GANs

## Overview
This project explores the application of **Generative Adversarial Networks (GANs)** across multiple domains including synthetic data, medical imaging, cybersecurity, and creative AI.

The objective is to understand how GANs learn data distributions and evaluate their effectiveness using both visual and quantitative methods.

---

## Project Objectives

- Implement GANs on synthetic datasets (Sine Wave, Mixture of Gaussians)
- Apply GANs to real-world datasets:
  - **BloodMNIST (Medical Imaging)**
  - **CICIDS 2017 (Cybersecurity)**
  - **QuickDraw (Creative AI)**
- Compare real and generated data distributions
- Evaluate performance using:
  - Visual analysis
  - Loss curves
  - Fréchet Inception Distance (FID)

---

## Project Structure
generative-modelling-gans-case-study/
├── README.md
├── requirements.txt
├── .gitignore
├── generative_modelling_case_study.ipynb
├── outputs/
│ ├── part1/
│ ├── bloodmnist/
│ ├── cicids/
│ └── quickdraw/
└── docs/
└── report_figures_note.md

---

## Datasets

### Synthetic Data
- Sine wave distribution  
- Mixture of Gaussians  

### BloodMNIST
- Source: MedMNIST  
- Task: Generate synthetic blood cell images  

### CICIDS 2017
- Source: Preprocessed CICIDS dataset  
- Task: Generate synthetic network traffic data  
- Focus: Wednesday subset (BENIGN and DoS attacks)  

### QuickDraw (Pizza)
- Source: Google QuickDraw dataset  
- Task: Generate synthetic sketch images  

---

## Methodology

### Part 1 – Synthetic Data
- MLP-based GAN  
- Learning simple and multi-modal distributions  
- Evaluation of mode collapse and architecture improvements  

### Part 2.1 – BloodMNIST
- DCGAN architecture  
- Image generation  
- Loss analysis and hyperparameter comparison  
- Evaluation using FID  

### Part 2.2 – CICIDS
- GAN applied to tabular data  
- PCA and t-SNE visualisation  
- Feature distribution comparison  

### Part 2.3 – QuickDraw
- DCGAN for sketch generation  
- Visual evaluation of generated samples  
- FID-based assessment  

---

## Key Findings
- GANs perform well on structured and image-based data  
- Strong results observed for:
  - Synthetic datasets  
  - BloodMNIST  
  - QuickDraw  
- Weak performance observed for:
  - CICIDS (tabular data)  
- Common challenges:
  - Mode collapse  
  - Training instability  
  - Limited diversity in generated samples  

---

## Evaluation Metric

### Fréchet Inception Distance (FID)
FID measures the similarity between real and generated image distributions.

- Lower FID indicates better quality  
- Used for BloodMNIST and QuickDraw  

---

## Computational Considerations
Due to computational constraints:
- Reduced dataset sizes were used  
- Limited training epochs were applied  
- FID was computed on smaller subsets  

Despite these limitations, the results effectively demonstrate GAN behaviour.

---

## How to Run

### Install dependencies
pip install -r requirements.txt

### Run the notebook
jupyter notebook generative_modelling_case_study.ipynb


---

## Outputs
The `outputs/` folder contains:
- Generated samples  
- Loss curves  
- Distribution comparisons  
- Evaluation visualisations  

These outputs are used in the final report.

---

## Notes
- Raw datasets are not included due to size limitations  
- The project is fully reproducible using the provided notebook and dependencies  

---

## Author
Salla Tarun Kumar  
MSc Data Science  
University of Hertfordshire  

---

## GitHub Repository
https://github.com/itzTarun219/generative-modelling-gans-case-study
