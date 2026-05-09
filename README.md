# HLA-DR4Pred: SVM-Based Method for Predicting HLA-DRB1*0401 Binding Peptides

Welcome to the official documentation for **HLA-DR4Pred**, a computational tool developed to predict HLA-DRB1*0401 binding peptides in an antigenic sequence. Identifying these peptides is essential for reducing the experimental workload required to find helper T-cell epitopes, which are crucial for vaccine design and understanding autoimmune diseases.

**Web Server:** [http://www.imtech.res.in/raghava/hladr4pred/](http://www.imtech.res.in/raghava/hladr4pred/)(https://webs.iiitd.edu.in/raghava/hladr4pred)

---

## Citation

Bhasin, M., & Raghava, G. P. S. (2004). 
**SVM based method for predicting HLA-DRB1*0401 binding peptides in an antigen sequence.** *Bioinformatics*, 20(3), 421-423. 
[https://doi.org/10.1093/bioinformatics/btg424](https://doi.org/10.1093/bioinformatics/btg424)

---

## About the Platform

The HLA-DR4Pred platform utilizes Support Vector Machines (SVM) to classify peptides as binders or non-binders for the HLA-DRB1*0401 allele. Unlike older motif-based methods, this SVM-based approach captures complex patterns in peptide sequences, leading to significantly higher prediction accuracy.

### Key Features
* **SVM-Light Implementation**: Developed using the SVM-light package, which is optimized for large-scale structural patterns.
* **High Accuracy**: Achieved an accuracy of 86% when evaluated through 5-fold cross-validation.
* **Large Dataset**: Trained on a clean dataset consisting of 567 known binders and 567 non-binders.

---

## Technical Overview

The performance of the method is based on the ability of the SVM to learn from the primary amino acid sequences of peptides.

| Metric | Value |
| :--- | :--- |
| **Training Set Size** | 1,134 peptides (567 binders, 567 non-binders) |
| **Accuracy** | 86% |
| **Validation Method** | 5-fold cross-validation |

---

## Model Functionality

HLA-DR4Pred allows users to scan an entire protein sequence to identify potential binding regions.

* **Sequence Input**: Users can submit single or multiple protein sequences in a standard format.
* **Adjustable Threshold**: Users can select different threshold values to balance sensitivity and specificity based on their research requirements.
* **Binder Identification**: The server identifies 9-mer core regions within the protein that are most likely to bind to the HLA-DRB1*0401 allele.

---

## Applications

* **Vaccine Design**: Identifying potential T-cell epitopes for the development of subunit vaccines.
* **Autoimmunity Research**: Scanning proteins for peptides that might trigger HLA-DRB1*0401-associated autoimmune responses.
* **Immunology**: Reducing the number of synthetic peptides required for experimental binding assays.

---

## Contact & Authors

**Manoj Bhasin** & **G. P. S. Raghava** Bioinformatics Centre, Institute of Microbial Technology, Sector 39A, Chandigarh, India.  
**Email**: raghava@imtech.res.in

---

## License

This project is an open-access resource and is available for academic use provided the original work is properly cited.
