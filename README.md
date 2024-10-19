# Structural Variants in Insulin Regulation: A Study on Neonatal Diabetes and Hyperinsulinism

## Overview

This repository contains the code and analysis for my dissertation project titled **"Structural Variants in Insulin Regulation: A Study on Neonatal Diabetes and Hyperinsulinism"**. The project explores the role of **Structural Variants (SVs)** in rare conditions such as **Neonatal Diabetes Mellitus (NDM)** and **Congenital Hyperinsulinism (CHI)**. These conditions affect the body's regulation of insulin, with NDM causing insufficient insulin production and CHI leading to excessive insulin secretion. The primary aim of the study is to identify overlapping **de novo** structural variants in individuals with NDM and CHI, which may uncover novel mechanisms of disease.

## Repository Contents

### 1. Data Cleaning (`Data_Cleaning.ipynb`)
This notebook contains the preprocessing steps for the dataset, including:
- Consolidation of raw data into a unified format
- Genotype assignment to detect inheritance patterns of variants
- Cleaning and standardization of genomic coordinates

### 2. Exploratory Analysis (`Exploratory_Analysis.ipynb`)
The exploratory analysis focuses on:
- Identifying the distribution of variant frequencies across samples
- Detecting outliers and potential sequencing errors
- Visualizing the distribution of genetic consequences (e.g., deletions, duplications, inversions)

### 3. Variant Filtering (`Filtering.ipynb`)
This notebook outlines the steps taken to filter out irrelevant or unreliable variants and focus on **de novo SVs**:
- Removal of unreliable variant calls (e.g., low read counts, large variants)
- Exclusion of common and non-causative variants
- Focus on variants occurring exclusively in genes potentially related to NDM and CHI

## Project Aim

The goal of the project is to leverage whole genome sequencing data to identify and validate **de novo structural variants** that could explain the genetic basis of **Neonatal Diabetes Mellitus** and **Congenital Hyperinsulinism**. By focusing on **high-confidence structural variants**, we aim to uncover novel pathways involved in insulin regulation.

### Key Findings
- The filtering process resulted in the identification of 20 candidate de novo SVs in the NDM cohort and 23 in the CHI cohort.
- Inversions were identified in the **IFITM** gene cluster, and deletions were found in **MTUS2**, suggesting potential novel genetic contributors to CHI.
- Further functional validation is required to confirm the contribution of these genes to the disease.

## Dissertation

The complete dissertation is available in the file **"700009050.pdf"**. It provides detailed background, methods, and results of the study, including:
- An overview of structural variant detection methods
- Detailed results of the exploratory analysis and variant filtering
- Discussion of the potential role of the **IFITM** gene cluster in insulin regulation
- Future directions for functional validation and research on machine learning approaches to variant analysis.

## Future Work

### 1. Functional Validation
- Further validation using **long-read sequencing** is required to confirm the identified structural variants.
- Techniques like **CRISPR/Cas9** and **single-cell RNA sequencing** are proposed to explore the functional consequences of the identified variants.

### 2. Machine Learning Approaches
- Future work could involve the integration of **machine learning** to improve variant calling and filtering, allowing for more accurate detection of SVs in large datasets.

## Installation

To run the notebooks, clone the repository and ensure you have the following dependencies:
- Python 3.x
- Jupyter
- Required Python libraries: `matplotlib`, `pandas`, `bedtools`, etc.

Install the dependencies using:
```bash
pip install -r requirements.txt
